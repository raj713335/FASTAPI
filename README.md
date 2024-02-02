## Start the FastAPI App

```commandline
uvicorn books:app --reload
```


## Swagger

```commandline
http://127.0.0.1:8000/docs
```

## Pydantic v1 vs Pydantic v2

FastAPI is now compatible with both Pydantic v1 and Pydantic v2.
Based on how new the version of FastAPI you are using, there could be small method name changes.


The three biggest are:
- .dict() function is now renamed to .model_dump()
- schema_extra function within a Config class is now renamed to json_schema_extra
- Optional variables need a =None example: id: Optional[int] = None

## SQL Queries
.mode table
INSERT INTO todos(title, description, priority, complete) VALUES ('Go to Store', 'To pick up eggs', 4, False);