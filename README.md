# Colleges Management

## Overview

created rest api for colleges management. And fetching them based upon courses.

## Architecture

- Controller
- Service
- Repository
- Models / Entities
- Data Insertion


## How to Run

1. Run the Spring Boot application.
2. Data is inserted into H2 database automatically or your mysql (change in application.properties).
3. Access H2 Console at [http://localhost:8080/h2-console](http://localhost:8080/h2-console).

## Endpoints

### fETCH ALL COLLEGES

- **URL:** `GET (http://localhost:8080/colleges/fetch-all-colleges)
- **Request Body:**
    [
    {
        "collegeId": "cee8ee17-b4bc-44ab-bc32-621d725d6e94",
        "collegeName": "Bvrit",
        "courseName": "java",
        "courseDuration": "2 months",
        "accomodation": "AC",
        "accomodationFee": 200,
        "courseFee": {
            "courseFee_id": "db3c3806-d9c1-48d9-8341-0d936cc8fd33",
            "fees": 3000
        }
    },
    {
        "collegeId": "bee4dd6b-27ef-4dc5-b633-5af771acac56",
        "collegeName": "iit",
        "courseName": "python",
        "courseDuration": "4 months",
        "accomodation": "non-AC",
        "accomodationFee": 340,
        "courseFee": {
            "courseFee_id": "aeb98d70-101b-4527-bc79-0845d943f4dc",
            "fees": 4000
        }
    }
    
  
]
    ```

  

## Entities

- Colleges
- CourseFee
