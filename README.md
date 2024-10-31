
---

# Junior Laravel Developer - Practical Test

### `Duration → max 24 hours `

# **Instruction**

1. **Read** the requirements in detail.
2. **Develop and upload** to your new public repo.
3. **Document** the following in your `README.md`:
   - How to set up the project locally (including migrations, seeders, and storage links).
   - How to run the project (include commands for serving and running tests).
   - How to interact with the API (if you completed the API endpoints).
4. **Send us** the repo URL back.
5. **Commit** 1st when you start and finish, so we can track time.

---

## Requirements

### **1. Authentication**
- `implement` **Basic Authentication** using Laravel Breeze or Jetstream (instead of the default `make:auth`).
- `ensure` **RBAC**: only users with the role of **Administrator** can manage companies and employees.
  - seed the database with an initial user:
    - Email: `admin@admin.com`
    - Password: `password`
    - Role: `Administrator`

### **2. CRUD**
- `implement` CRUD operations for two models: **Company** and **Employee**.

#### **Companies:**
- `name`, `email`, `logo`, `website`

#### **Employees:**
- `name`, `email`, `phone`, `profile`, `company_id`

### **3. Additional Features:**
1. **File Handling for Logos and Profiles:**
   - `store` images in the `storage/app/public` directory.
   - `ensure` they are accessible via a public URL `/storage`.
   - `resize` uploaded logos automatically to ensure they meet the minimum (100X100) and maximum (600x600) requirement.
   - `use` Laravel Image Processing, e.g., `intervention/image`.

2. **Implement Eloquent Relationships**
   - Set up relationships between the `Company` and `Employee` models.
   - A company can have many employees; an employee belongs to one company.

3. **Search and Pagination:**
   - Implement search on `name` and `email` fields for both `Company` and `Employee`.
   - Use Laravel’s pagination to display the list of Companies and Employees.

6. **Documentation Skill:**
   - Provide clear setup instructions in the `README.md`.
   - Describe any additional setup or usage notes.

### **4. API Endpoints (Bonus Task)**
- `create` **RESTful API** endpoints for managing companies and employees:
  - `GET /api/companies`
  - `POST /api/companies`
  - `PUT /api/companies/{id}`
  - `DELETE /api/companies/{id}`
- `use` **API Token Authentication** (Laravel Passport or Sanctum)
- `ensure` proper error handling and validation for each API endpoint

---

### **Expected Skills**

- Coding Proficiency
- Basic Understanding of Laravel Framework
- Best practices for authentication and file handling
- Documentation Skill
- **Bonus**: API development and documentation

### **Notes**

- This project is not for business flows. You don't need to consider for that.
- This project is intended for **Coding Skill** only.
- You have to write meaningful git commits.
- You can improve your code as much as you can, **we will consider as bonus points**.