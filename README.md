# 🎓 Student REST API - Spring Boot Application

This is a simple Spring Boot REST API that manages student data. It allows you to retrieve student information, filter by age, sort by GPA, and fetch specific students by registration number.

# Sample data

```bash
Student s1 = new Student("2020ICT31", "Ruwini", 24, "IT", 3.79);
Student s2 = new Student("2020ASP29", "Ilma", 23, "CS", 3.80);
Student s3 = new Student("2020BIO91", "Dilmy", 22, "BIO", 3.43);
Student s4 = new Student("2020ICT47", "Maleesha", 24, "IT", 3.66);
Student s5 = new Student("2020BS85", "Kasun", 25, "BS", 3.87);

```

# API Endpoints

#### 1. Display 'Hello SpringBoot!' message.

Endpoint: 
```bash
  http://localhost:8080/app/msg
```
Response:
```bash
  Hello SpringBoot!
```
Output: 
![Screenshot (474)](https://github.com/user-attachments/assets/097ec33a-a7cf-4568-9065-fd1d6016c8f6)


# 
#### 2. Display a message with user provided age.

Endpoint: 
```bash
  http://localhost:8080/app/age/24
```
Response:
```bash
  My age is 24
```
Output:
![Screenshot (468)](https://github.com/user-attachments/assets/a7320f2b-b7a3-40e8-bda1-412f6c1af1c0)


# 
#### 3. Return a particular student.

Endpoint: 
```bash
  http://localhost:8080/app/student
```
Response:
```bash
    {
        "regNo": "2020ICT31",
        "name": "Ruwini",
        "age": 24,
        "course": "IT",
        "gpa": 3.79
    }
```
Output:
![Screenshot (469)](https://github.com/user-attachments/assets/6a67a5b6-c41a-412a-8041-c340b895bc79)


# 
#### 4. Return multiple students.

Endpoint: 
```bash
  http://localhost:8080/app/students
```
Response:
```bash
[
    {
        "regNo": "2020ICT31",
        "name": "Ruwini",
        "age": 24,
        "course": "IT",
        "gpa": 3.79
    },
    {
        "regNo": "2020ASP29",
        "name": "Ilma",
        "age": 23,
        "course": "CS",
        "gpa": 3.8
    },
    {
        "regNo": "2020BIO91",
        "name": "Dilmy",
        "age": 22,
        "course": "BIO",
        "gpa": 3.43
    },
    {
        "regNo": "2020ICT47",
        "name": "Maleesha",
        "age": 24,
        "course": "IT",
        "gpa": 3.66
    },
    {
        "regNo": "2020BS85",
        "name": "Kasun",
        "age": 25,
        "course": "BS",
        "gpa": 3.87
    }
]
```
Output:
![Screenshot (470)](https://github.com/user-attachments/assets/87739abd-8ad9-44b0-adef-91126d5a4269)


# 
#### 5. return a student by regNo.

Endpoint: 
```bash
  http://localhost:8080/app/students/2020BIO91
```
Response:
```bash
    {
        "regNo": "2020BIO91",
        "name": "Dilmy",
        "age": 22,
        "course": "BIO",
        "gpa": 3.43
    }
```
Output:
![Screenshot (471)](https://github.com/user-attachments/assets/348a6097-2ab6-4936-97de-52882c69ffb2)


# 
#### 6. Return students whose age is between 20-23

Endpoint: 
```bash
  http://localhost:8080/app/agebetween20-23
```
Response:
```bash
[
    {
        "regNo": "2020ASP29",
        "name": "Ilma",
        "age": 23,
        "course": "CS",
        "gpa": 3.8
    },
    {
        "regNo": "2020BIO91",
        "name": "Dilmy",
        "age": 22,
        "course": "BIO",
        "gpa": 3.43
    }
]
```
Output:
![Screenshot (472)](https://github.com/user-attachments/assets/2ebba347-395b-4505-b12e-1223592ce9df)


# 
#### 7. Sort students by their gpa

Endpoint: 
```bash
  http://localhost:8080/app/students/gpa
```
Response:
```bash
[
    {
        "regNo": "2020BIO91",
        "name": "Dilmy",
        "age": 22,
        "course": "BIO",
        "gpa": 3.43
    },
    {
        "regNo": "2020ICT47",
        "name": "Maleesha",
        "age": 24,
        "course": "IT",
        "gpa": 3.66
    },
    {
        "regNo": "2020ICT31",
        "name": "Ruwini",
        "age": 24,
        "course": "IT",
        "gpa": 3.79
    },
    {
        "regNo": "2020ASP29",
        "name": "Ilma",
        "age": 23,
        "course": "CS",
        "gpa": 3.8
    },
    {
        "regNo": "2020BS85",
        "name": "Kasun",
        "age": 25,
        "course": "BS",
        "gpa": 3.87
    }
]
```
Output:
![Screenshot (473)](https://github.com/user-attachments/assets/44715def-4706-4f0b-8aeb-190371f365ad)

