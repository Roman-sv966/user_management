
# User Management - Final Project

## Project Overview
The **User Management System** is a robust platform designed to manage user profiles, roles, and account features effectively. It includes functionalities like enhanced profile management, bug resolutions, and CI/CD improvements. This project follows industry best practices, enabling a strong foundation for real-world applications.

---

## Key Features ✨

### 1. **Enhanced Profile Update Functionality**
- **Description**: Improved user profile management with support for profile picture updates and extended user fields.
- **Issue Resolved**: [#11](https://github.com/Roman-sv966/user_management/issues/11)

### 2. **Email Verification Process Fixes**
- **Issue**: During email verification, `user-id` was found to be `None`, causing failures.
- **Resolution**: Added checks to ensure `user-id` is validated before verification.
- **Issue Reference**: [#7](https://github.com/Roman-sv966/user_management/issues/7)

### 3. **Schema Update for Professional Status**
- **Issue**: The `is_professional` field was missing from the schema and response object.
- **Resolution**: Included the missing field and updated the response models.
- **Issue Reference**: [#9](https://github.com/Roman-sv966/user_management/issues/9)

 **Bug Fixes and System Stabilization**
### 4. **Incorrect Role Assignment**: Fixed the issue of incorrect role downgrades during admin email verification ([#5](https://github.com/Roman-sv966/user_management/issues/5)).
### 5. **Dependency Conflicts**: Resolved FastAPI-Starlette version conflicts causing service crashes ([#3](https://github.com/Roman-sv966/user_management/issues/3)).
### 6. **Docker Build Failures**: Fixed `apt-get` installation errors for specific `libc-bin` versions during builds ([#1](https://github.com/Roman-sv966/user_management/issues/1)).

---

## Enhancements 🛠️
- **Security Improvements**: Resolved high and critical vulnerabilities in Python dependencies ([#2](https://github.com/Roman-sv966/user_management/issues/2)).
- **CI/CD Integration**: Ensured smooth Docker builds and enhanced deployment pipelines.

---

## Installation Instructions ⚙️

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/Roman-sv966/user_management.git
   cd user_management
   ```

2. **Set Up Environment**:
   - Install dependencies:
     ```bash
     pip install -r requirements.txt
     ```

3. **Run Services with Docker**:
   ```bash
   docker-compose up --build
   ```

4. **Access the Application**:
   - FastAPI Docs: [http://localhost/docs](http://localhost/docs)
   - Application: [http://localhost](http://localhost)

---

## Testing 🔍

To run tests:
```bash
pytest tests/
```

---

## Project Links 🔗
- **GitHub Repository**: [User Management System](https://github.com/Roman-sv966/user_management)
- **Closed Issues**:
   - [#11](https://github.com/Roman-sv966/user_management/issues/11): Enhanced Profile Update
   - [#9](https://github.com/Roman-sv966/user_management/issues/9): Missing is_professional Field
   - [#7](https://github.com/Roman-sv966/user_management/issues/7): Email Verification Fix
   - [#5](https://github.com/Roman-sv966/user_management/issues/5): Role Assignment Fix
   - [#3](https://github.com/Roman-sv966/user_management/issues/3): FastAPI-Starlette Dependency Conflict
   - [#2](https://github.com/Roman-sv966/user_management/issues/2): Critical Python Vulnerabilities
   - [#1](https://github.com/Roman-sv966/user_management/issues/1): Docker Build Issue
- **DockerHub**: [[DockerHub Link](https://hub.docker.com/r/sv966/user_management)]

---

## Contributors 👨‍💻
- **Roman-sv966**

---

## License 📄
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## Future Improvements 🚧
- Implement advanced role-based access control.
- Enhance search capabilities with additional filters.
- Add API rate-limiting for improved security.
