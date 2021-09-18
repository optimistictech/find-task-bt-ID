## Find task by ID

### Description
 This returns a single task
 
###  Endpoint
*/task/{id}*

### Http request method
*GET*
 
### Parameters(Request queries)
| ID         | Data type | Description            |
| -----------| --------- | ---------------------- |
| task_id    | string    | ID of the task         |

### Responses
 - Successful operation
 - Description: Returns task by ID
 - Status code: 200
 - Response body:  
     
     ```sh
      {
        "_id": "string",
        "user_id": "string",
        "title": "doggie",
        "description": "string",
        "status": "pending",
        "start_date": "string",
        "end_date": "string",
        "deleted_date": "string",
        "archive_at": "string",
        "recurring_data": {},
        "labels": "string",
        "collaborators": [
        "string"
        ]
    }
    ```
- Invalid request
  - Description: Invalid ID supplied 
  
    - Status code: 400
    
  - Task not found
  
    - Status code: 404

