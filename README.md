# Colleges Management

## Overview

Created REST API for colleges management. Fetching colleges based on the courses they offer.

## Architecture

- Controller
- Service
- Repository
- Models / Entities
- Data Insertion

## How to Run

1. Run the Spring Boot application.
2. Data is inserted into the H2 database automatically or your MySQL (change in `application.properties`).
3. Access H2 Console at [http://localhost:8080/h2-console](http://localhost:8080/h2-console).

## Endpoints

### Fetch All Colleges

- **URL**: `GET http://localhost:8080/colleges/fetch-all-colleges`
- **Response Body**:
    ```json
    [
        {
            "collegeId": "cee8ee17-b4bc-44ab-bc32-621d725d6e94",
            "collegeName": "Bvrit",
            "courseName": "java",
            "courseDuration": "2 months",
            "accommodation": "AC",
            "accommodationFee": 200,
            "courseFee": {
                "courseFee_id": "db3c3806-d9c1-48d9-8341-0d936cc8fd33",
                "fees": 3000
            }
        },
        {
            "collegeId": "bee4dd6b-27ef-4dc5-b633-5af771acac56",
            "collegeName": "IIT",
            "courseName": "python",
            "courseDuration": "4 months",
            "accommodation": "non-AC",
            "accommodationFee": 340,
            "courseFee": {
                "courseFee_id": "aeb98d70-101b-4527-bc79-0845d943f4dc",
                "fees": 4000
            }
        }
    ]
    ```

## Entities

- **Colleges**
- **CourseFee**
