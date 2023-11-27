# RABC

## 理念

权限设计思想

<!-- [代码示例](/Users/hanwenhao/NodeProjects/rbac) -->

角色基于访问控制（RBAC：Role-Based Access Control）是一种常见的权限管理方法，其核心思想是用户通过角色与权限关联。这样，不必直接给用户分配权限，而是分配角色给用户，角色再关联具备的权限。以下是一个基于RBAC思想的MySQL数据库表结构示例：

```mysql
-- 用户（users）表：
CREATE TABLE users (
  user_id INT AUTO_INCREMENT PRIMARY KEY,
  username VARCHAR(50) NOT NULL UNIQUE,
  password_hash VARCHAR(255) NOT NULL,
  email VARCHAR(100),
  status TINYINT NOT NULL DEFAULT 1, -- 用于表示用户状态，如激活、禁用等
  created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
  updated_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP ON UPDATE CURRENT_TIMESTAMP
);

-- 角色（roles）表：
CREATE TABLE roles (
  role_id INT AUTO_INCREMENT PRIMARY KEY,
  role_name VARCHAR(50) NOT NULL UNIQUE,
  description VARCHAR(255),
  created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
  updated_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP ON UPDATE CURRENT_TIMESTAMP
);

-- 权限（permissions）表：
CREATE TABLE permissions (
  permission_id INT AUTO_INCREMENT PRIMARY KEY,
  permission_name VARCHAR(50) NOT NULL UNIQUE,
  description VARCHAR(255)
);

-- 用户角色关联（user_roles）表：
CREATE TABLE user_roles (
  user_id INT,
  role_id INT,
  PRIMARY KEY (user_id, role_id),
  FOREIGN KEY (user_id) REFERENCES users(user_id) ON DELETE CASCADE,
  FOREIGN KEY (role_id) REFERENCES roles(role_id) ON DELETE CASCADE
);

-- 角色权限关联（role_permissions）表：
CREATE TABLE role_permissions (
  role_id INT,
  permission_id INT,
  PRIMARY KEY (role_id, permission_id),
  FOREIGN KEY (role_id) REFERENCES roles(role_id) ON DELETE CASCADE,
  FOREIGN KEY (permission_id) REFERENCES permissions(permission_id) ON DELETE CASCADE
);

```

这个结构为每个用户定义了一或多个角色，每个角色则具备了一或多个权限。对于RBAC系统来说，会有更多细节需要管理，比如管理角色之间的继承关系等，但以上表结构为这些关系提供了一个良好的起点。用户可通过自己的角色来获得相应的权限，进行相关的操作。
