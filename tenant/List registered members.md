# Pre condition

* Tenant member must exists in CP

# Endpoint

```
POST http://localhost:30000/api/v1/tenants/members/registered/search
```

## Responses

### Success

* Status 200 OK

| Object | Fields | Data Type | Note | 
| --- | --- | --- | --- |
| JSON Object | \- | \- | Response Payload | 
| \- | data | \[\]Member | \- | 
| Member | \- | \- | Tenant member | 
| \- | id | string | Tenant member ID | 
| \- | display_name | string | tenant_users.display_name from Navis | 
| \- | email | string | tenant_users.email from Navis | 
| \- | roles | \[\]string | Tenant member roles | 

# Payload

POST http://localhost:30000/api/v1/tenants/members/registered/search

# Response

## Success

* Status 200 OK

```
{
    "data": [
        {
            "id": "12dsf213123",
            "display_name": "CaptainAmerica1",
            "email": "do.thi.hoai.nho@moneyforward.vn",
            "roles": [
                "submitter",
                "administrator
            ]
        }
    ]
}
```
