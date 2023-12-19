## API Gateway
- **Swagger**
  ```yaml
    ---
  swagger: "2.0"
  info:
    version: "1.0.0"
    title: "Pet Adoption API"
  host: "b8gke3dl56.execute-api.us-east-1.amazonaws.com"
  basePath: "/test"
  schemes:
  - "https"
  paths:
    /Pets:
      get:
        produces:
        - "application/json"
        responses:
          "200":
            description: "200 response"
    /adopter/create:
      post:
        produces:
        - "application/json"
        responses:
          "200":
            description: "200 response"
    /adopter/{adopter_id}:
      get:
        produces:
        - "application/json"
        parameters:
        - name: "adopter_id"
          in: "path"
          required: true
          type: "string"
        responses:
          "200":
            description: "200 response"
      put:
        produces:
        - "application/json"
        parameters:
        - name: "adopter_id"
          in: "path"
          required: true
          type: "string"
        responses:
          "200":
            description: "200 response"
      delete:
        produces:
        - "application/json"
        parameters:
        - name: "adopter_id"
          in: "path"
          required: true
          type: "string"
        responses:
          "200":
            description: "200 response"
    /adopters:
      get:
        produces:
        - "application/json"
        responses:
          "200":
            description: "200 response"
    /create:
      post:
        produces:
        - "application/json"
        responses:
          "200":
            description: "200 response"
    /createpetowner:
      post:
        produces:
        - "application/json"
        responses:
          "200":
            description: "200 response"
    /delete/{id}:
      delete:
        produces:
        - "application/json"
        parameters:
        - name: "id"
          in: "path"
          required: true
          type: "string"
        responses:
          "200":
            description: "200 response"
    /deletepetowner/{id}:
      delete:
        produces:
        - "application/json"
        parameters:
        - name: "id"
          in: "path"
          required: true
          type: "string"
        responses:
          "200":
            description: "200 response"
    /getowner/{id}:
      get:
        produces:
        - "application/json"
        parameters:
        - name: "id"
          in: "path"
          required: true
          type: "string"
        responses:
          "200":
            description: "200 response"
    /update_to_white/{id}:
      put:
        produces:
        - "application/json"
        parameters:
        - name: "id"
          in: "path"
          required: true
          type: "string"
        responses:
          "200":
            description: "200 response"
    /updatepetowner/{id}:
      put:
        produces:
        - "application/json"
        parameters:
        - name: "id"
          in: "path"
          required: true
          type: "string"
        responses:
          "200":
            description: "200 response"
  ```
- **Lambda Integration**:
  <img width="975" alt="Screenshot 2023-12-16 at 8 57 38 PM" src="https://github.com/SteveJu/COMS6156UI/assets/98562104/caa9e008-5bb0-4b93-b9e6-ee738e5375d0">

## Auth-Middleware
AWS Cognito (to-do)

## S3 Front-end Static Website
- **URL**: http://6156-frontend.s3-website-us-east-1.amazonaws.com


