# api
API Docs

FORMAT: 1A
HOST: https://crm.EXAMPLE.com/


# Stockton Api Docs

Welcome to the **API Documentation V6**! You can use our API to access **CRM API** endpoints, for information about various positions, tickets, leads campaigns etc. in our database.

In this document we will survey how to access, and use the API.

The following pages will contain examples of common usages of the API, a complete revision of the API Modules, code examples, and other important information.
## Note
**This document is under constant work, so if you feel that something important is missing, or if you notice something is incorrect,
feel free to contact us at support@Stockton.**

## Data Endpoints [/]

### List Common Data [GET /api/v5/options]

Retrieves countries, languages, currencies etc. You are able to use it in upcoming requests.


+ Response 200 (application/json)

        {
            "data": []
          }
        }    
    

### List All Avaialble Terms [GET /api/v6/terms{?token}]

All available terms with possible fields and conditions.

+ Parameters
    + token: `YOUR_TOKEN_HERE`  (required, text) ... Your secret token for auth


+ Response 200 (application/json)

        {
            "data": []
          }
        }    
    
    
### List All Avaialble Actions [GET /api/v6/actions{?token}]

All available actions with methods signature.

+ Parameters
    + token: `YOUR_TOKEN_HERE`  (required, text) ... Your secret token for auth
 
+ Response 200 (application/json)

        {
            "data": []
          }
        }    
        

## Terms [/api/v6/terms]

### List All Traders [GET /api/v6/terms/Traders{?token,perPage,page}]

Retrieves all Traders which linked to him.

**NOTE:** Trader should be linked to you by registering with correct token for getting results.

+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    + perPage: `1` (optional, number) ... How many items per page
        + Default: `15`
    + page: `1` (optional, number) ... What page should be loaded
    
+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### List All Transactions [GET /api/v6/terms/Transactions{?token,perPage,page}]

Retrieves all Transactions which linked to him.

**NOTE:** Trader should be linked to you by registering with correct token for getting results.

+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    + perPage: `1` (optional, number) ... How many items per page
        + Default: `15`
    + page: `1` (optional, number) ... What page should be loaded
    
+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### List All DepositTickets [GET /api/v6/terms/DepositTickets{?token,perPage,page}]

Retrieves all DepositTickets which linked to him.

**NOTE:** Trader should be linked to you by registering with correct token for getting results.

+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    + perPage: `1` (optional, number) ... How many items per page
        + Default: `15`
    + page: `1` (optional, number) ... What page should be loaded
    
+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### List All WithdrawalTickets [GET /api/v6/terms/WithdrawalTickets{?token,perPage,page}]

Retrieves all WithdrawalTickets which linked to him.

**NOTE:** Trader should be linked to you by registering with correct token for getting results.

+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    + perPage: `1` (optional, number) ... How many items per page
        + Default: `15`
    + page: `1` (optional, number) ... What page should be loaded
    
+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### List All ChargeBacks [GET /api/v6/terms/ChargeBacks{?token,perPage,page}]

Retrieves all ChargeBacks which linked to him.

**NOTE:** Trader should be linked to you by registering with correct token for getting results.

+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    + perPage: `1` (optional, number) ... How many items per page
        + Default: `15`
    + page: `1` (optional, number) ... What page should be loaded
    
+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### List All Positions [GET /api/v6/terms/Positions{?token,perPage,page}]

Retrieves all Positions which linked to him.

**NOTE:** Trader should be linked to you by registering with correct token for getting results.

+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    + perPage: `1` (optional, number) ... How many items per page
        + Default: `15`
    + page: `1` (optional, number) ... What page should be loaded
    
+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### List All Workers [GET /api/v6/terms/Workers{?token,perPage,page}]

Retrieves all Workers which linked to him.

**NOTE:** Trader should be linked to you by registering with correct token for getting results.

+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    + perPage: `1` (optional, number) ... How many items per page
        + Default: `15`
    + page: `1` (optional, number) ... What page should be loaded
    
+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### List All Desks [GET /api/v6/terms/Desks{?token,perPage,page}]

Retrieves all Desks which linked to him.

**NOTE:** Trader should be linked to you by registering with correct token for getting results.

+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    + perPage: `1` (optional, number) ... How many items per page
        + Default: `15`
    + page: `1` (optional, number) ... What page should be loaded
    
+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### List All Campaigns [GET /api/v6/terms/Campaigns{?token,perPage,page}]

Retrieves all Campaigns which linked to him.

**NOTE:** Trader should be linked to you by registering with correct token for getting results.

+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    + perPage: `1` (optional, number) ... How many items per page
        + Default: `15`
    + page: `1` (optional, number) ... What page should be loaded
    
+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### List All TradingGroups [GET /api/v6/terms/TradingGroups{?token,perPage,page}]

Retrieves all TradingGroups which linked to him.

**NOTE:** Trader should be linked to you by registering with correct token for getting results.

+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    + perPage: `1` (optional, number) ... How many items per page
        + Default: `15`
    + page: `1` (optional, number) ... What page should be loaded
    
+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### List All WorkerActions [GET /api/v6/terms/WorkerActions{?token,perPage,page}]

Retrieves all WorkerActions which linked to him.

**NOTE:** Trader should be linked to you by registering with correct token for getting results.

+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    + perPage: `1` (optional, number) ... How many items per page
        + Default: `15`
    + page: `1` (optional, number) ... What page should be loaded
    
+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### List All FTD Traders [GET /api/v6/terms/Traders{?token,perPage,page,conditions[]}]

Retrieves all Traders with FTD which linked to him.

**NOTE:** Trader should be linked to you by registering with correct token for getting results.

+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    + perPage: `1` (optional, number) ... How many items per page
        + Default: `15`
    + page: `1` (optional, number) ... What page should be loaded
    + conditions: `conditions[0][name]=customers.ftd_date,conditions[0][operator]=in+date+range,conditions[0][value]=2018-01-25+00:00:00+-+2020-12-30+23:59:59` (optional, array) ... Conditions
    
+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }
        
### List All FTD DepositTickets [GET /api/v6/terms/DepositTickets{?token,perPage,page,conditions[]}]

Retrieves all Deposits with FTD status which linked to him.

**NOTE:** Trader should be linked to you by registering with correct token for getting results.

+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    + perPage: `1` (optional, number) ... How many items per page
        + Default: `15`
    + page: `1` (optional, number) ... What page should be loaded
    + conditions: `conditions[0][key]=tickets.is_ftd,conditions[0][operator]==,conditions[0][value]=1,conditions[1][key]=customers.campaign_id,conditions[1][operator]==,conditions[1][value]=5` (optional, array) ... Conditions
    
+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }
    
    
    
    

## Customer Actions [/api/v6/terms/Customer/]


### CreateAndLogin [POST /api/v6/action/Customer/CreateAndLogin/execute/{?token}]

Most recomended for client registration.
Redirect the client to the autologin url it returns 


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + arguments
            + fname: `-` (required, string) - Enter your new customer first name (required, string, min:1, max:26)
            + lname: `-` (required, string) - Enter your new customer last name (required, string, min:1, max:26)
            + street: `-` (required, string) - Enter customer address (required, string, min:1, max:60)
            + city: `-` (required, string) - Enter customer city (required, string, min:1, max:26)
            + country: `-` (required, string) - Choice country from list (required, string, from list)
            + currency: `-` (required, string) - Change currency (required, string, from list)
            + email: `-` (required, string) - Enter email address (required, string, min:1, max:80)
            + fax: `-` (required, string) - Enter fax number
            + language: `-` (required, string) - Choice language from list (required, string, from list)
            + mobile: `-` (required, string) - Enter your new trader mobile (required, string)
            + password: `-` (required, string) - Enter password (required, string, min:1, max:80)
            + email_send: `-` (required, string) - Send email notification? (required, integer:"1"/"0")
            + phone: `-` (required, string) - Enter your new trader phone (required, string)
            + state: `-` (required, string) - Enter customer state (required, string, min:1, max:26)
            + campaign_id: `-` (required, string) - Choose campaign (required, exists)
            + employee_id: `-` (required, string) - Choose employee (required, exists)
            + desk_id: `-` (required, string) - Choose desk (required, exists)
            + trading_group_id: `-` (required, string) - Choose trading group (required, exists)
            + broker_employee_id: `-` (required, string) - Choose broker employee (required, exists)
            + ip_address: `-` (required, string) - IP address of client (required, exists)
            + a_aid: `-` (required, string) - Extra details of campaign (required, exists)
            + b_bid: `-` (required, string) - Extra details of campaign (required, exists)
            + sub_brand `-` (optional, string) - Extra details of target brand (optional, exists)
            + redirect_page: '-' /#/crypto-wallet/deposit/request'


+ Response 200 (application/json)

        {
            "status": "something"
            "url": "https.." // redirect to that
            "object_id": xxx // customer ID
        }  

### CreateNew [POST /api/v6/action/Customer/CreateNew/execute/{?token}]

Action from Customer namespace, short description - Create new customer.

Arguments:

```json
[
    {
        "type": "Text",
        "name": "fname",
        "description": "Enter your new customer first name"
    },
    {
        "type": "Text",
        "name": "lname",
        "description": "Enter your new customer last name"
    },
    {
        "type": "Text",
        "name": "street",
        "description": "Enter customer address"
    },
    {
        "type": "Text",
        "name": "city",
        "description": "Enter customer city"
    },
    {
        "type": "Select",
        "name": "country",
        "description": "Choice country from list"
    },
    {
        "type": "Select",
        "name": "currency",
        "description": "Change currency"
    },
    {
        "type": "Text",
        "name": "email",
        "description": "Enter email address"
    },
    {
        "type": "Text",
        "name": "fax",
        "description": "Enter fax number"
    },
    {
        "type": "Select",
        "name": "language",
        "description": "Choice language from list"
    },
    {
        "type": "Text",
        "name": "mobile",
        "description": "Enter your new trader mobile"
    },
    {
        "type": "Password",
        "name": "password",
        "description": "Enter password"
    },
    {
        "type": "Select",
        "name": "email_send",
        "description": "Send email notification?"
    },
    {
        "type": "Text",
        "name": "phone",
        "description": "Enter your new trader phone"
    },
    {
        "type": "Text",
        "name": "state",
        "description": "Enter customer state"
    },
    {
        "type": "Select",
        "name": "campaign_id",
        "description": "Choose campaign"
    },
    {
        "type": "Select",
        "name": "sub_source",
        "description": "Choose sub source"
    },
    {
        "type": "Select",
        "name": "sub_source2",
        "description": "Choose sub source"
    },
    {
        "type": "Select",
        "name": "sub_source3",
        "description": "Choose sub source"
    },
    {
        "type": "Select",
        "name": "sub_source4",
        "description": "Choose sub source"
    },
    {
        "type": "Select",
        "name": "sub_brand",
        "description": "Choose sub brand"
    },
    {
        "type": "Select",
        "name": "sub_source5",
        "description": "Choose sub source"
    },

    {
        "type": "Select",
        "name": "employee_id",
        "description": "Choose employee"
    },
    {
        "type": "Select",
        "name": "desk_id",
        "description": "Choose desk"
    },
    {
        "type": "Select",
        "name": "trading_group_id",
        "description": "Choose trading group"
    },
    {
        "type": "Select",
        "name": "broker_employee_id",
        "description": "Choose broker employee"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[fname]=something

- attributes[lname]=something

- attributes[street]=something

- attributes[city]=something

- attributes[country]=something

- attributes[currency]=something

- attributes[email]=something

- attributes[fax]=something

- attributes[language]=something

- attributes[mobile]=something

- attributes[password]=something

- attributes[email_send]=something

- attributes[phone]=something

- attributes[state]=something

- attributes[campaign_id]=something

- attributes[sub_source]=something
- attributes[sub_source2]=something 
- attributes[sub_source3]=something 
- attributes[sub_source4]=something 
- attributes[sub_source5]=something 

- attributes[sub_brand]=something 

- attributes[employee_id]=something

- attributes[desk_id]=something

- attributes[trading_group_id]=something

- attributes[broker_employee_id]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + fname: `-` (required, string) - Enter your new customer first name (required, string, min:1, max:26)
        + lname: `-` (required, string) - Enter your new customer last name (required, string, min:1, max:26)
        + street: `-` (required, string) - Enter customer address (required, string, min:1, max:60)
        + city: `-` (required, string) - Enter customer city (required, string, min:1, max:26)
        + country: `-` (required, string) - Choice country from list (required, string, from list)
        + currency: `-` (required, string) - Change currency (required, string, from list)
        + email: `-` (required, string) - Enter email address (required, string, min:1, max:80)
        + fax: `-` (required, string) - Enter fax number
        + language: `-` (required, string) - Choice language from list (required, string, from list)
        + mobile: `-` (required, string) - Enter your new trader mobile (required, string)
        + password: `-` (required, string) - Enter password (required, string, min:1, max:80)
        + email_send: `-` (required, string) - Send email notification? (required, integer:"1"/"0")
        + phone: `-` (required, string) - Enter your new trader phone (required, string)
        + state: `-` (required, string) - Enter customer state (required, string, min:1, max:26)
        + campaign_id: `-` (required, string) - Choose campaign (required, exists)
        + employee_id: `-` (required, string) - Choose employee (required, exists)
        + desk_id: `-` (required, string) - Choose desk (required, exists)
        + trading_group_id: `-` (required, string) - Choose trading group (required, exists)
        + broker_employee_id: `-` (required, string) - Choose broker employee (required, exists)
        + ip_address: `-` (required, string) - IP address of client (required, exists)
        + a_aid: `-` (required, string) - Extra details of campaign (required, exists)
        + b_bid: `-` (required, string) - Extra details of campaign (required, exists)
        + sub_brand `-` (optional, string) - Extra details of target brand (optional, exists)



+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }        
        
### Edit [POST /api/v6/action/Customer/Edit/execute/1{?token,perPage,page}]

Action from Customer namespace, short description - Edit the customer.

Arguments:

```json
[
    {
        "type": "Text",
        "name": "fname",
        "description": "Enter your new customer first name"
    },
    {
        "type": "Text",
        "name": "lname",
        "description": "Enter your new customer last name"
    },
    {
        "type": "Text",
        "name": "street",
        "description": "Enter customer address"
    },
    {
        "type": "Text",
        "name": "city",
        "description": "Enter customer city"
    },
    {
        "type": "Select",
        "name": "country",
        "description": "Choice country from list"
    },
    {
        "type": "Select",
        "name": "currency",
        "description": "Change currency"
    },
    {
        "type": "Text",
        "name": "email",
        "description": "Enter email address"
    },
    {
        "type": "Text",
        "name": "fax",
        "description": "Enter fax number"
    },
    {
        "type": "Select",
        "name": "language",
        "description": "Choice language from list"
    },
    {
        "type": "Text",
        "name": "mobile",
        "description": "Enter your new trader mobile"
    },
    {
        "type": "Text",
        "name": "phone",
        "description": "Enter your new trader phone"
    },
    {
        "type": "Text",
        "name": "state",
        "description": "Enter customer state"
    }
    {
        "type": "Select",
        "name": "sub_brand",
        "description": "Choose sub brand"
    },
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[fname]=something

- attributes[lname]=something

- attributes[street]=something

- attributes[city]=something

- attributes[country]=something

- attributes[currency]=something

- attributes[email]=something

- attributes[fax]=something

- attributes[language]=something

- attributes[mobile]=something

- attributes[phone]=something

- attributes[state]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + fname: `-` (required, string) - Enter your new customer first name
        + lname: `-` (required, string) - Enter your new customer last name
        + street: `-` (required, string) - Enter customer address
        + city: `-` (required, string) - Enter customer city
        + country: `-` (required, string) - Choice country from list
        + currency: `-` (required, string) - Change currency
        + email: `-` (required, string) - Enter email address
        + fax: `-` (required, string) - Enter fax number
        + language: `-` (required, string) - Choice language from list
        + mobile: `-` (required, string) - Enter your new trader mobile
        + phone: `-` (required, string) - Enter your new trader phone
        + state: `-` (required, string) - Enter customer state


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }        
        
### Get JWT token [POST /api/v6/action/Customer/GetJwtToken/execute/{user_id}{?token}]

Action from Customer namespace, short description - Get the link to login with JWT.

Arguments:

```json
[
    {
        "type": "String",
        "name": "page",
        "description": "Page to redirect (for example, '/#!/pl-fb/account/deposit/request')"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[page]=something

+ Parameters
    + user_id: `ID of user` (required, integer) ... Your User ID
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth

+ Response 200 (application/json)

        {
          "url": "http://example.com/signin/jwt-token/<JWT_TOKEN>"
        }        
        



### AddDocument [POST /api/v6/action/Customer/AddDocument/execute/1{?token,perPage,page}]

Action from Customer namespace, short description - Add Document To Trader.

Arguments:

```json
[
    {
        "type": "Text",
        "name": "name",
        "description": "Title of Document"
    },
    {
        "type": "File",
        "name": "file",
        "description": "Select DOcument"
    },
    {
        "type": "String",
        "name": "category",
        "description": "Select Category"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[name]=something

- attributes[file]=something

- attributes[category]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + name: `-` (required, string) - Title of Document
        + file: `-` (required, string) - Select Document  
        + category: `-` (required, string) - Select Category


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### AddBonus [GET /api/v6/action/Customer/AddBonus/execute/1{?token,perPage,page}]

Action from Customer namespace, short description - Add Bonus.

Arguments:

```json
[
    {
        "type": "Number",
        "name": "amount",
        "description": "Amount of bonus"
    },
    {
        "type": "Number",
        "name": "leverage",
        "description": "Leverage amount"
    },
    {
        "type": "Text",
        "name": "description",
        "description": "A reason for adding a bonus"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[amount]=something

- attributes[leverage]=something

- attributes[description]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + amount: `-` (required, string) - Amount of bonus
        + leverage: `-` (required, string) - Leverage amount
        + description: `-` (required, string) - A reason for adding a bonus  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### AddRemark [GET /api/v6/action/Customer/AddRemark/execute/1{?token,perPage,page}]

Action from Customer namespace, short description - Add Remark.

Arguments:

```json
[
    {
        "type": "File",
        "name": "customer",
        "description": "Empty"
    },
    {
        "type": "Select",
        "name": "priority",
        "description": "Priority of Remark"
    },
    {
        "type": "Select",
        "name": "status",
        "description": "Status of Remark"
    },
    {
        "type": "Text",
        "name": "title",
        "description": "Title of Remark"
    },
    {
        "type": "TextArea",
        "name": "message",
        "description": "Message of Remark"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[customer]=something

- attributes[priority]=something

- attributes[status]=something

- attributes[title]=something

- attributes[message]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + customer: `-` (required, string) - Empty
        + priority: `-` (required, string) - Priority of Remark
        + status: `-` (required, string) - Status of Remark
        + title: `-` (required, string) - Title of Remark
        + message: `-` (required, string) - Message of Remark  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### AddManualDeposit [POST /api/v6/action/Customer/AddManualDeposit/execute{?token,perPage,page}]

Action from Customer namespace, short description - Create Deposit Ticket.

Arguments:

```json
[
    {
        "type": "Number",
        "name": "amount",
        "description": "Amount of deposit"
    },
    {
        "type": "Autocomplete",
        "name": "method",
        "description": "Select type of deposit"
    },
    {
        "type": "Text",
        "name": "description",
        "description": "A reason for adding a deposit"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[amount]=something

- attributes[method]=something

- attributes[description]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + amount: `-` (required, string) - Amount of deposit
        + method: `-` (required, string) - Select type of deposit
        + description: `-` (required, string) - A reason for adding a deposit  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### AddManualTicketDeposit [GET /api/v6/action/Customer/AddManualTicketDeposit/execute/1{?token,perPage,page}]

Action from Customer namespace, short description - Create Deposit Ticket.

Arguments:

```json
[
    {
        "type": "Number",
        "name": "amount",
        "description": "Amount"
    },
    {
        "type": "Select",
        "name": "method",
        "description": "Method"
    },
    {
        "type": "Text",
        "name": "description",
        "description": "Description"
    },
    {
        "type": "Text",
        "name": "transaction_id",
        "description": "Provider transaction ID (not required)"
    },
    {
        "type": "String",
        "name": "created_at_date",
        "description": "Created At Date"
    },
    {
        "type": "String",
        "name": "created_at_time",
        "description": "Created At Time"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[amount]=something

- attributes[method]=something

- attributes[description]=something

- attributes[transaction_id]=something

- attributes[created_at_date]=something

- attributes[created_at_time]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + amount: `-` (required, string) - Amount
        + method: `-` (required, string) - Method
        + description: `-` (required, string) - Description
        + transaction_id: `-` (required, string) - Provider transaction ID (not required)
        + created_at_date: `-` (required, string) - Created At Date  
        + created_at: `-` (required, string) - Created At Time


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### AddManualTicketWithdrawal [GET /api/v6/action/Customer/AddManualTicketWithdrawal/execute/1{?token,perPage,page}]

Action from Customer namespace, short description - Create Withdrawal Ticket.

Arguments:

```json
[
    {
        "type": "Number",
        "name": "amount",
        "description": "Amount"
    },
    {
        "type": "Select",
        "name": "method",
        "description": "Method"
    },
    {
        "type": "Text",
        "name": "description",
        "description": "Description"
    },
    {
        "type": "DateTime",
        "name": "created_at",
        "description": "Created at"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[amount]=something

- attributes[method]=something

- attributes[description]=something

- attributes[created_at]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + amount: `-` (required, string) - Amount
        + method: `-` (required, string) - Method
        + description: `-` (required, string) - Description
        + created_at: `-` (required, string) - Created at  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### AddManualWireDeposit [GET /api/v6/action/Customer/AddManualWireDeposit/execute/1{?token,perPage,page}]

Action from Customer namespace, short description - Create Wire Deposit.

Arguments:

```json
[
    {
        "type": "Number",
        "name": "amount",
        "description": "Amount"
    },
    {
        "type": "Text",
        "name": "bank_name",
        "description": "Bank Name"
    },
    {
        "type": "Text",
        "name": "bank_number",
        "description": "Bank Number"
    },
    {
        "type": "Text",
        "name": "account_number",
        "description": "Account Number"
    },
    {
        "type": "Text",
        "name": "branch_number",
        "description": "Branch Number"
    },
    {
        "type": "Text",
        "name": "iban_bic_number",
        "description": "IBAN\/BIC"
    },
    {
        "type": "Text",
        "name": "bank_confirmation_code",
        "description": "Confirmation Code"
    },
    {
        "type": "Text",
        "name": "description",
        "description": "Description"
    },
    {
        "type": "DateTime",
        "name": "created_at",
        "description": "Created at"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[amount]=something

- attributes[bank_name]=something

- attributes[bank_number]=something

- attributes[account_number]=something

- attributes[branch_number]=something

- attributes[iban_bic_number]=something

- attributes[bank_confirmation_code]=something

- attributes[description]=something

- attributes[created_at]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + amount: `-` (required, string) - Amount
        + bank_name: `-` (required, string) - Bank Name
        + bank_number: `-` (required, string) - Bank Number
        + account_number: `-` (required, string) - Account Number
        + branch_number: `-` (required, string) - Branch Number
        + iban_bic_number: `-` (required, string) - IBAN/BIC
        + bank_confirmation_code: `-` (required, string) - Confirmation Code
        + description: `-` (required, string) - Description
        + created_at: `-` (required, string) - Created at  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### AddTerminalDeposit [GET /api/v6/action/Customer/AddTerminalDeposit/execute/1{?token,perPage,page}]

Action from Customer namespace, short description - Create Terminal Deposit.

Arguments:

```json
[
    {
        "type": "Number",
        "name": "amount",
        "description": "Amount of deposit"
    },
    {
        "type": "Select",
        "name": "method",
        "description": "Choice method for deposit"
    },
    {
        "type": "Text",
        "name": "email",
        "description": "Email"
    },
    {
        "type": "Text",
        "name": "fname",
        "description": "First Name"
    },
    {
        "type": "Text",
        "name": "lname",
        "description": "lname"
    },
    {
        "type": "File",
        "name": "ip_address",
        "description": "Empty"
    },
    {
        "type": "Select",
        "name": "country",
        "description": "Choice country for deposit"
    },
    {
        "type": "Text",
        "name": "city",
        "description": "City"
    },
    {
        "type": "Text",
        "name": "street",
        "description": "Street"
    },
    {
        "type": "Text",
        "name": "postal",
        "description": "Postal"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[amount]=something

- attributes[method]=something

- attributes[email]=something

- attributes[fname]=something

- attributes[lname]=something

- attributes[ip_address]=something

- attributes[country]=something

- attributes[city]=something

- attributes[street]=something

- attributes[postal]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + amount: `-` (required, string) - Amount of deposit
        + method: `-` (required, string) - Choice method for deposit
        + email: `-` (required, string) - Email
        + fname: `-` (required, string) - First Name
        + lname: `-` (required, string) - lname
        + ip_address: `-` (required, string) - Empty
        + country: `-` (required, string) - Choice country for deposit
        + city: `-` (required, string) - City
        + street: `-` (required, string) - Street
        + postal: `-` (required, string) - Postal  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### AssignNewDesk [GET /api/v6/action/Customer/AssignNewDesk/execute/1{?token,perPage,page}]

Action from Customer namespace, short description - Change Desk.

Arguments:

```json
[
    {
        "type": "Select",
        "name": "desk_id",
        "description": "Choice desk from list"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[desk_id]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + desk_id: `-` (required, string) - Choice desk from list  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### BlockLogin [GET /api/v6/action/Customer/BlockLogin/execute/1{?token,perPage,page}]

Action from Customer namespace, short description - Block trader login.

Arguments:

```json
[]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:




+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
          


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### EditPassword [GET /api/v6/action/Customer/EditPassword/execute/1{?token,perPage,page}]

Action from Customer namespace, short description - Edit password.

Arguments:

```json
[
    {
        "type": "Password",
        "name": "password",
        "description": "Enter password"
    },
    {
        "type": "Select",
        "name": "email_send",
        "description": "Send email notification?"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[password]=something

- attributes[email_send]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + password: `-` (required, string) - Enter password
        + email_send: `-` (required, string) - Send email notification?  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### RefreshAccount [GET /api/v6/action/Customer/RefreshAccount/execute/1{?token,perPage,page}]

Action from Customer namespace, short description - Refresh account.

Arguments:

```json
[]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:




+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
          


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### ChangeBroker [GET /api/v6/action/Customer/ChangeBroker/execute/1{?token,perPage,page}]

Action from Customer namespace, short description - Change broker.

Arguments:

```json
[
    {
        "type": "Select",
        "name": "employee_id",
        "description": "Choose broker"
    },
    {
        "type": "Select",
        "name": "self_status",
        "description": "Choose sale status"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[employee_id]=something

- attributes[self_status]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + employee_id: `-` (required, string) - Choose broker
        + self_status: `-` (required, string) - Choose sale status  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### ChangeCampaign [GET /api/v6/action/Customer/ChangeCampaign/execute/1{?token,perPage,page}]

Action from Customer namespace, short description - Change Campaign.

Arguments:

```json
[
    {
        "type": "Select",
        "name": "campaign_id",
        "description": "Choose campaign"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[campaign_id]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + campaign_id: `-` (required, string) - Choose campaign  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### ChangeSalestatus [GET /api/v6/action/Customer/ChangeSalestatus/execute/1{?token,perPage,page}]

Action from Customer namespace, short description - Change sale status.

Arguments:

```json
[
    {
        "type": "Select",
        "name": "self_status",
        "description": "Choose sale status"
    },
    {
        "type": "TextArea",
        "name": "create_communication",
        "description": "Create communication?"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[self_status]=something

- attributes[create_communication]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + self_status: `-` (required, string) - Choose sale status
        + create_communication: `-` (required, string) - Create communication?  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### ChangeSegment [GET /api/v6/action/Customer/ChangeSegment/execute/1{?token,perPage,page}]

Action from Customer namespace, short description - Change segment.

Arguments:

```json
[
    {
        "type": "Select",
        "name": "segment",
        "description": "Choose segment"
    },
    {
        "type": "TextArea",
        "name": "create_communication",
        "description": "Create communication?"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[segment]=something

- attributes[create_communication]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + segment: `-` (required, string) - Choose segment
        + create_communication: `-` (required, string) - Create communication?  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### ChangeValidationStatus [GET /api/v6/action/Customer/ChangeValidationStatus/execute/1{?token,perPage,page}]

Action from Customer namespace, short description - Change verification status.

Arguments:

```json
[
    {
        "type": "Select",
        "name": "validation_status",
        "description": "Choose validation status"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[validation_status]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + validation_status: `-` (required, string) - Choose validation status  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### CreateCallHistory [GET /api/v6/action/Customer/CreateCallHistory/execute/1{?token,perPage,page}]

Action from Customer namespace, short description - Create Call History.

Arguments:

```json
[
    {
        "type": "Text",
        "name": "title",
        "description": "Select method of title"
    },
    {
        "type": "TextArea",
        "name": "description",
        "description": "Enter description"
    },
    {
        "type": "Select",
        "name": "self_status",
        "description": "Choose sale status"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[title]=something

- attributes[description]=something

- attributes[self_status]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + title: `-` (required, string) - Select method of title
        + description: `-` (required, string) - Enter description
        + self_status: `-` (required, string) - Choose sale status  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### CreateChargeBack [POST /api/v6/action/Customer/CreateChargeBack/execute{?token,perPage,page}]

Action from Customer namespace, short description - Create Charge Back.

Arguments:

```json
[
    {
        "type": "Select",
        "name": "deposit_id",
        "description": "Choose deposit"
    },
    {
        "type": "String",
        "name": "created_at_date",
        "description": "Created At Date"
    },
    {
        "type": "String",
        "name": "created_at_time",
        "description": "Created At Time"
    }
]
```

**NOTE:** Data should be represented as arguments[name], instead of raw JSON.

For example like this:

- arguments[deposit_id]=something

- arguments[created_at_date]=something

- arguments[created_at_time]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + deposit_id: `-` (required, string) - Choose deposit
        + created_at_date: `-` (required, string) - Created At Date
        + created_at_time: `-` (required, string) - Created At Time


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### EditAddress [GET /api/v6/action/Customer/EditAddress/execute/1{?token,perPage,page}]

Action from Customer namespace, short description - Edit customer address.

Arguments:

```json
[
    {
        "type": "Text",
        "name": "street",
        "description": "Enter customer address"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[street]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + street: `-` (required, string) - Enter customer address  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### EditCity [GET /api/v6/action/Customer/EditCity/execute/1{?token,perPage,page}]

Action from Customer namespace, short description - Edit customer city.

Arguments:

```json
[
    {
        "type": "Text",
        "name": "city",
        "description": "Enter customer city"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[city]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + city: `-` (required, string) - Enter customer city  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### EditCountry [GET /api/v6/action/Customer/EditCountry/execute/1{?token,perPage,page}]

Action from Customer namespace, short description - Edit country for trader.

Arguments:

```json
[
    {
        "type": "Select",
        "name": "country",
        "description": "Choice country from list"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[country]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + country: `-` (required, string) - Choice country from list  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### EditCurrency [GET /api/v6/action/Customer/EditCurrency/execute/1{?token,perPage,page}]

Action from Customer namespace, short description - Change currency.

Arguments:

```json
[
    {
        "type": "Select",
        "name": "currency",
        "description": "Change currency"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[currency]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + currency: `-` (required, string) - Change currency  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### EditFName [GET /api/v6/action/Customer/EditFName/execute/1{?token,perPage,page}]

Action from Customer namespace, short description - Edit customer first name.

Arguments:

```json
[
    {
        "type": "Text",
        "name": "fname",
        "description": "Enter your new customer first name"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[fname]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + fname: `-` (required, string) - Enter your new customer first name  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### EditFax [GET /api/v6/action/Customer/EditFax/execute/1{?token,perPage,page}]

Action from Customer namespace, short description - Edit fax number.

Arguments:

```json
[
    {
        "type": "Text",
        "name": "fax",
        "description": "Enter fax number"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[fax]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + fax: `-` (required, string) - Enter fax number  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### EditLName [GET /api/v6/action/Customer/EditLName/execute/1{?token,perPage,page}]

Action from Customer namespace, short description - Edit trader last name.

Arguments:

```json
[
    {
        "type": "Text",
        "name": "lname",
        "description": "Enter your new customer last name"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[lname]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + lname: `-` (required, string) - Enter your new customer last name  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### EditLanguage [GET /api/v6/action/Customer/EditLanguage/execute/1{?token,perPage,page}]

Action from Customer namespace, short description - Edit language for trader.

Arguments:

```json
[
    {
        "type": "Select",
        "name": "language",
        "description": "Choice language from list"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[language]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + language: `-` (required, string) - Choice language from list  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### EditMobile [GET /api/v6/action/Customer/EditMobile/execute/1{?token,perPage,page}]

Action from Customer namespace, short description - Edit mobile phone for trader.

Arguments:

```json
[
    {
        "type": "Text",
        "name": "mobile",
        "description": "Enter your new trader mobile"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[mobile]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + mobile: `-` (required, string) - Enter your new trader mobile  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### EditPhone [GET /api/v6/action/Customer/EditPhone/execute/1{?token,perPage,page}]

Action from Customer namespace, short description - Edit phone for trader.

Arguments:

```json
[
    {
        "type": "Text",
        "name": "phone",
        "description": "Enter your new trader phone"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[phone]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + phone: `-` (required, string) - Enter your new trader phone  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### EditEmail [GET /api/v6/action/Customer/EditEmail/execute/1{?token,perPage,page}]

Action from Customer namespace, short description - Edit email address.

Arguments:

```json
[
    {
        "type": "Text",
        "name": "email",
        "description": "Enter email address"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[email]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + email: `-` (required, string) - Enter email address  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### EditRegistrationStatus [GET /api/v6/action/Customer/EditRegistrationStatus/execute/1{?token,perPage,page}]

Action from Customer namespace, short description - Remove Registration Status.

Arguments:

```json
[]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:




+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
          


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### EditState [GET /api/v6/action/Customer/EditState/execute/1{?token,perPage,page}]

Action from Customer namespace, short description - Edit customer state.

Arguments:

```json
[
    {
        "type": "Text",
        "name": "state",
        "description": "Enter customer state"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[state]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + state: `-` (required, string) - Enter customer state  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### ForceStrategy [GET /api/v6/action/Customer/ForceStrategy/execute/1{?token,perPage,page}]

Action from Customer namespace, short description - Force Strategy.

Arguments:

```json
[
    {
        "type": "Text",
        "name": "forced_strategy",
        "description": "Enter your number"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[forced_strategy]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + forced_strategy: `-` (required, string) - Enter your number  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### UnBlockLogin [GET /api/v6/action/Customer/UnBlockLogin/execute/1{?token,perPage,page}]

Action from Customer namespace, short description - Unblock trader login.

Arguments:

```json
[]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:




+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
          


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### UnBlockTrading [GET /api/v6/action/Customer/UnBlockTrading/execute/1{?token,perPage,page}]

Action from Customer namespace, short description - Unblock trader trading.

Arguments:

```json
[]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:




+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
          


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### BlockTrading [GET /api/v6/action/Customer/BlockTrading/execute/1{?token,perPage,page}]

Action from Customer namespace, short description - Block trader trading.

Arguments:

```json
[]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:




+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
          


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### SendNotify [GET /api/v6/action/Customer/SendNotify/execute/1{?token,perPage,page}]

Action from Customer namespace, short description - Send Push Notification.

Arguments:

```json
[
    {
        "type": "Text",
        "name": "message",
        "description": "Enter message"
    },
    {
        "type": "File",
        "name": "template",
        "description": "Empty"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[message]=something

- attributes[template]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + message: `-` (required, string) - Enter message
        + template: `-` (required, string) - Empty  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### ChangeAffiliate [GET /api/v6/action/Customer/ChangeAffiliate/execute/1{?token,perPage,page}]

Action from Customer namespace, short description - Change affiliate.

Arguments:

```json
[
    {
        "type": "Select",
        "name": "employee_id",
        "description": "Choose affiliate"
    },
    {
        "type": "Select",
        "name": "self_status",
        "description": "Choose sale status"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[employee_id]=something

- attributes[self_status]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + employee_id: `-` (required, string) - Choose affiliate
        + self_status: `-` (required, string) - Choose sale status  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### AssignNewTradingGroup [GET /api/v6/action/Customer/AssignNewTradingGroup/execute/1{?token,perPage,page}]

Action from Customer namespace, short description - Assign new trading group.

Arguments:

```json
[
    {
        "type": "Select",
        "name": "trading_group_id",
        "description": "Choice trading group from list"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[trading_group_id]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + trading_group_id: `-` (required, string) - Choice trading group from list  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### CreateHyperPosition [GET /api/v6/action/Customer/CreateHyperPosition/execute/1{?token,perPage,page}]

Action from Customer namespace, short description - Open Hyper Position.

Arguments:

```json
[
    {
        "type": "WatchedSelect",
        "name": "position_asset_id",
        "description": "Choice asset from the list"
    },
    {
        "type": "LinkedSelect",
        "name": "position_expiration",
        "description": "Choice expiration"
    },
    {
        "type": "Number",
        "name": "position_amount",
        "description": "Amount of position"
    },
    {
        "type": "Select",
        "name": "position_type",
        "description": "Choice direction"
    },
    {
        "type": "Number",
        "name": "position_forced_strategy",
        "description": "Trading Strategy"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[position_asset_id]=something

- attributes[position_expiration]=something

- attributes[position_amount]=something

- attributes[position_type]=something

- attributes[position_forced_strategy]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + position_asset_id: `-` (required, string) - Choice asset from the list
        + position_expiration: `-` (required, string) - Choice expiration
        + position_amount: `-` (required, string) - Amount of position
        + position_type: `-` (required, string) - Choice direction
        + position_forced_strategy: `-` (required, string) - Trading Strategy  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### CreateRegularTermPosition [GET /api/v6/action/Customer/CreateRegularTermPosition/execute/1{?token,perPage,page}]

Action from Customer namespace, short description - Open Regular Term Position.

Arguments:

```json
[
    {
        "type": "WatchedSelect",
        "name": "position_asset_id",
        "description": "Choice asset from the list"
    },
    {
        "type": "LinkedSelect",
        "name": "position_option_id",
        "description": "Choice option"
    },
    {
        "type": "Number",
        "name": "position_amount",
        "description": "Amount of position"
    },
    {
        "type": "Select",
        "name": "position_type",
        "description": "Choice direction"
    },
    {
        "type": "Number",
        "name": "position_forced_strategy",
        "description": "Trading Strategy"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[position_asset_id]=something

- attributes[position_option_id]=something

- attributes[position_amount]=something

- attributes[position_type]=something

- attributes[position_forced_strategy]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + position_asset_id: `-` (required, string) - Choice asset from the list
        + position_option_id: `-` (required, string) - Choice option
        + position_amount: `-` (required, string) - Amount of position
        + position_type: `-` (required, string) - Choice direction
        + position_forced_strategy: `-` (required, string) - Trading Strategy  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### ExportCalls [GET /api/v6/action/Customer/ExportCalls/execute/1{?token,perPage,page}]

Action from Customer namespace, short description - Export calls.

Arguments:

```json
[]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:




+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
          


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### ExportPositions [GET /api/v6/action/Customer/ExportPositions/execute/1{?token,perPage,page}]

Action from Customer namespace, short description - Export positions.

Arguments:

```json
[]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:




+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
          


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### ExportTransactions [GET /api/v6/action/Customer/ExportTransactions/execute/1{?token,perPage,page}]

Action from Customer namespace, short description - Export transactions.

Arguments:

```json
[]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:




+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
          


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### ExportLogins [GET /api/v6/action/Customer/ExportLogins/execute/1{?token,perPage,page}]

Action from Customer namespace, short description - Export logins.

Arguments:

```json
[]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:




+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
          


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### SendEmail [GET /api/v6/action/Customer/SendEmail/execute/1{?token,perPage,page}]

Action from Customer namespace, short description - Send Email By Template.

Arguments:

```json
[
    {
        "type": "Text",
        "name": "subject",
        "description": "Subject"
    },
    {
        "type": "Select",
        "name": "template",
        "description": "Email template"
    },
    {
        "type": "Select",
        "name": "account",
        "description": "Email account"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[subject]=something

- attributes[template]=something

- attributes[account]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + subject: `-` (required, string) - Subject
        + template: `-` (required, string) - Email template
        + account: `-` (required, string) - Email account  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### VoiceSpinCall [GET /api/v6/action/Customer/VoiceSpinCall/execute/1{?token,perPage,page}]

Action from Customer namespace, short description - Dial trader.

Arguments:

```json
[
    {
        "type": "Select",
        "name": "number",
        "description": "Select the number"
    },
    {
        "type": "Select",
        "name": "prefix",
        "description": "Select the prefix"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[number]=something

- attributes[prefix]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + number: `-` (required, string) - Select the number
        + prefix: `-` (required, string) - Select the prefix  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### ConvertToCustomer [GET /api/v6/action/Customer/ConvertToCustomer/execute/1{?token,perPage,page}]

Action from Customer namespace, short description - Convert to Customer.

Arguments:

```json
[
    {
        "type": "Text",
        "name": "password",
        "description": "Password"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[password]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + password: `-` (required, string) - Password  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }
    
    
    
    
## Configuration Actions [/api/v6/terms/Configuration/]

### CreateDepartment [GET /api/v6/action/Configuration/CreateDepartment/execute/1{?token,perPage,page}]

Action from Configuration namespace, short description - Create Department.

Arguments:

```json
[
    {
        "type": "Select",
        "name": "parent_department",
        "description": "Select parent department"
    },
    {
        "type": "Text",
        "name": "value",
        "description": "Department Name"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[parent_department]=something

- attributes[value]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + parent_department: `-` (required, string) - Select parent department
        + value: `-` (required, string) - Department Name  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### DeleteDepartment [GET /api/v6/action/Configuration/DeleteDepartment/execute/1{?token,perPage,page}]

Action from Configuration namespace, short description - Delete Department.

Arguments:

```json
[
    {
        "type": "string",
        "name": "group",
        "description": "Name of department"
    },
    {
        "type": "string",
        "name": "value",
        "description": "Accept string (always 'Yes')"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[group]=something

- attributes[value]="Yes"


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + group: `-` (required, string) - Name of department
        + value: `Yes` (required, string) - Accept string (always "Yes")


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### EditField [GET /api/v6/action/Configuration/EditField/execute/1{?token,perPage,page}]

Action from Configuration namespace, short description - Edit field.

Arguments:

```json
[
    {
        "type": "Text",
        "name": "value",
        "description": "value"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[value]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + value: `-` (required, string) - value  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### EditMailTemplateField [GET /api/v6/action/Configuration/EditMailTemplateField/execute/1{?token,perPage,page}]

Action from Configuration namespace, short description - Edit email template field.

Arguments:

```json
[
    {
        "type": "Select",
        "name": "value",
        "description": "Choice email template"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[value]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + value: `-` (required, string) - Choice email template  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### CreateSegment [GET /api/v6/action/Configuration/CreateSegment/execute/1{?token,perPage,page}]

Action from Configuration namespace, short description - Create new segment.

Arguments:

```json
[
    {
        "type": "Text",
        "name": "name",
        "description": "Name"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[name]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + name: `-` (required, string) - Name  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### CreateSaleStatus [GET /api/v6/action/Configuration/CreateSaleStatus/execute/1{?token,perPage,page}]

Action from Configuration namespace, short description - Create new sale status.

Arguments:

```json
[
    {
        "type": "Text",
        "name": "name",
        "description": "Name"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[name]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + name: `-` (required, string) - Name  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### DeleteSaleStatus [GET /api/v6/action/Configuration/DeleteSaleStatus/execute/1{?token,perPage,page}]

Action from Configuration namespace, short description - Delete sale status.

Arguments:

```json
[
    {
        "type": "Select",
        "name": "name",
        "description": "Choose sale status which will be set to current sale status customers"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[name]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + name: `-` (required, string) - Choose sale status which will be set to current sale status customers  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### DeleteSegment [GET /api/v6/action/Configuration/DeleteSegment/execute/1{?token,perPage,page}]

Action from Configuration namespace, short description - Delete segment.

Arguments:

```json
[
    {
        "type": "Select",
        "name": "name",
        "description": "Choose segment which will be set to current segment customers"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[name]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + name: `-` (required, string) - Choose segment which will be set to current segment customers  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }


## SecurityApi Actions [/api/v6/terms/SecurityApi/]

### CreateNew [GET /api/v6/action/SecurityApi/CreateNew/execute/1{?token,perPage,page}]

Action from SecurityApi namespace, short description - Create new token user.

Arguments:

```json
[
    {
        "type": "Select",
        "name": "employee_id",
        "description": "Choose worker"
    },
    {
        "type": "Text",
        "name": "ips",
        "description": "Whitelisted IPs - separate with comma (ie. 80.442.124.1,135.34.65.1)"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[employee_id]=something

- attributes[ips]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, string) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + employee_id: `-` (required, string) - Choose worker
        + ips: `80.442.124.1,135.34.65.1` (required, string) - Whitelisted IPs - separate with comma


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### ChangeWorker [GET /api/v6/action/SecurityApi/ChangeWorker/execute/1{?token,perPage,page}]

Action from SecurityApi namespace, short description - Change worker.

Arguments:

```json
[
    {
        "type": "Select",
        "name": "employee_id",
        "description": "Choose worker"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[employee_id]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + employee_id: `-` (required, string) - Choose worker  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### Delete [GET /api/v6/action/SecurityApi/Delete/execute/1{?token,perPage,page}]

Action from SecurityApi namespace, short description - Delete Security Api.

Arguments:

```json
[
    {
        "type": "Text",
        "name": "value",
        "description": "Accept string (always 'Yes')"
    },
    {
        "type": "String",
        "name": "ids",
        "description": "Empty (separate with comma)"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[value]=something

- attributes[ids]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + value: `Yes` (required, string) - Accept string (always 'Yes')
        + ids: `-` (required, string) - Empty (separate with comma)


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### ChangeIp [GET /api/v6/action/SecurityApi/ChangeIp/execute/1{?token,perPage,page}]

Action from SecurityApi namespace, short description - Change IP API user.

Arguments:

```json
[
    {
        "type": "Text",
        "name": "ips",
        "description": "Whitelisted IPs - separate with comma (ie. 80.442.124.1,135.34.65.1)"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[ips]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + ips: `80.442.124.1,135.34.65.1` (required, string) - Whitelisted IPs - separate with comma (ie. 80.442.124.1,135.34.65.1)


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }


## Ip Actions [/api/v6/terms/Ip/]

### CreateNew [GET /api/v6/action/Ip/CreateNew/execute/1{?token,perPage,page}]

Action from Ip namespace, short description - Add New Whitelisted IP.

Arguments:

```json
[
    {
        "type": "Text",
        "name": "ips",
        "description": "Enter ip which will get access to CRM"
    },
    {
        "type": "Text",
        "name": "description",
        "description": "Enter description for ip"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[ip]=something

- attributes[description]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + ip: `-` (required, string) - Enter ip which will get access to crm
        + description: `-` (required, string) - Enter description for ip  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### Edit [GET /api/v6/action/Ip/Edit/execute/1{?token,perPage,page}]

Action from Ip namespace, short description - Edit ip.

Arguments:

```json
[
    {
        "type": "Text",
        "name": "ip",
        "description": "Enter ip which will get access to crm"
    },
    {
        "type": "Text",
        "name": "description",
        "description": "Enter description for ip"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[ip]=something

- attributes[description]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + ip: `-` (required, string) - Enter ip which will get access to crm
        + description: `-` (required, string) - Enter description for ip  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### EditDescription [GET /api/v6/action/Ip/EditDescription/execute/1{?token,perPage,page}]

Action from Ip namespace, short description - Edit description.

Arguments:

```json
[
    {
        "type": "Text",
        "name": "description",
        "description": "Enter description for ip"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[description]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + description: `-` (required, string) - Enter description for ip  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### EditIp [GET /api/v6/action/Ip/EditIp/execute/1{?token,perPage,page}]

Action from Ip namespace, short description - Edit ip address.

Arguments:

```json
[
    {
        "type": "Text",
        "name": "ip",
        "description": "Enter ip which will get access to crm"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[ip]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + ip: `-` (required, string) - Enter ip which will get access to crm  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }


## Campaign Actions [/api/v6/terms/Campaign/]

### Activate [GET /api/v6/action/Campaign/Activate/execute/1{?token,perPage,page}]

Action from Campaign namespace, short description - Activate campaign.

Arguments:

```json
[]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:




+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
          


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### CreateNew [GET /api/v6/action/Campaign/CreateNew/execute/1{?token,perPage,page}]

Action from Campaign namespace, short description - Create new campaign.

Arguments:

```json
[
    {
        "type": "Text",
        "name": "name",
        "description": "Choose name"
    },
    {
        "type": "Select",
        "name": "creator",
        "description": "Choose creator"
    },
    {
        "type": "Select",
        "name": "type",
        "description": "Choose calculation type"
    },
    {
        "type": "Number",
        "name": "timeout",
        "description": "Choose cookie timeout"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[name]=something

- attributes[creator]=something

- attributes[type]=something

- attributes[timeout]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + name: `-` (required, string) - Choose name
        + creator: `-` (required, string) - Choose creator
        + type: `-` (required, string) - Choose calculation type
        + timeout: `-` (required, string) - Choose cookie timeout  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### Deactivate [GET /api/v6/action/Campaign/Deactivate/execute/1{?token,perPage,page}]

Action from Campaign namespace, short description - Deactivate campaign.

Arguments:

```json
[]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:




+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
          


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### Edit [GET /api/v6/action/Campaign/Edit/execute/1{?token,perPage,page}]

Action from Campaign namespace, short description - Edit campaign.

Arguments:

```json
[
    {
        "type": "Text",
        "name": "name",
        "description": "Choose name"
    },
    {
        "type": "Select",
        "name": "creator",
        "description": "Choose creator"
    },
    {
        "type": "Select",
        "name": "type",
        "description": "Choose calculation type"
    },
    {
        "type": "Number",
        "name": "timeout",
        "description": "Choose cookie timeout"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[name]=something

- attributes[creator]=something

- attributes[type]=something

- attributes[timeout]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + name: `-` (required, string) - Choose name
        + creator: `-` (required, string) - Choose creator
        + type: `-` (required, string) - Choose calculation type
        + timeout: `-` (required, string) - Choose cookie timeout  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### EditCreator [GET /api/v6/action/Campaign/EditCreator/execute/1{?token,perPage,page}]

Action from Campaign namespace, short description - Edit campaign creator.

Arguments:

```json
[
    {
        "type": "Select",
        "name": "creator",
        "description": "Choose creator"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[creator]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + creator: `-` (required, string) - Choose creator  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### EditName [GET /api/v6/action/Campaign/EditName/execute/1{?token,perPage,page}]

Action from Campaign namespace, short description - Edit campaign name.

Arguments:

```json
[
    {
        "type": "Text",
        "name": "name",
        "description": "Choose name"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[name]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + name: `-` (required, string) - Choose name  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### EditTimeout [GET /api/v6/action/Campaign/EditTimeout/execute/1{?token,perPage,page}]

Action from Campaign namespace, short description - Edit campaign timeout.

Arguments:

```json
[
    {
        "type": "Number",
        "name": "timeout",
        "description": "Choose cookie timeout"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[timeout]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + timeout: `-` (required, string) - Choose cookie timeout  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### EditType [GET /api/v6/action/Campaign/EditType/execute/1{?token,perPage,page}]

Action from Campaign namespace, short description - Edit campaign type.

Arguments:

```json
[
    {
        "type": "Select",
        "name": "type",
        "description": "Choose calculation type"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[type]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + type: `-` (required, string) - Choose calculation type  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### AttachAffiliate [GET /api/v6/action/Campaign/AttachAffiliate/execute/1{?token,perPage,page}]

Action from Campaign namespace, short description - Attach Affiliate.

Arguments:

```json
[
    {
        "type": "Select",
        "name": "affiliate",
        "description": "Choose affiliate to attach"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[affiliate]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + affiliate: `-` (required, string) - Choose affiliate to attach  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### DetachAffiliate [GET /api/v6/action/Campaign/DetachAffiliate/execute/1{?token,perPage,page}]

Action from Campaign namespace, short description - Detach Affiliate.

Arguments:

```json
[
    {
        "type": "Select",
        "name": "affiliate",
        "description": "Choose affiliate to attach"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[affiliate]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + affiliate: `-` (required, string) - Choose affiliate to attach  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### Duplicate [GET /api/v6/action/Campaign/Duplicate/execute/1{?token,perPage,page}]

Action from Campaign namespace, short description - Duplicate Campaign.

Arguments:

```json
[]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:




+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
          


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }


## Tracker Actions [/api/v6/terms/Tracker/]

### CreateNew [GET /api/v6/action/Tracker/CreateNew/execute/1{?token,perPage,page}]

Action from Tracker namespace, short description - Create new tracker.

Arguments:

```json
[
    {
        "type": "File",
        "name": "type",
        "description": "Empty"
    },
    {
        "type": "File",
        "name": "campaign_id",
        "description": "Empty"
    },
    {
        "type": "Text",
        "name": "name",
        "description": "Enter tracker name"
    },
    {
        "type": "File",
        "name": "settings",
        "description": "Empty"
    },
    {
        "type": "Select",
        "name": "creator_id",
        "description": "Choose affiliate"
    },
    {
        "type": "Text",
        "name": "fire",
        "description": "Fire URL"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[type]=something

- attributes[campaign_id]=something

- attributes[name]=something

- attributes[settings]=something

- attributes[creator_id]=something

- attributes[fire]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + type: `-` (required, string) - Empty
        + campaign_id: `-` (required, string) - Empty
        + name: `-` (required, string) - Enter tracker name
        + settings: `-` (required, string) - Empty
        + creator_id: `-` (required, string) - Choose affiliate
        + fire: `-` (required, string) - Fire URL  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### Edit [GET /api/v6/action/Tracker/Edit/execute/1{?token,perPage,page}]

Action from Tracker namespace, short description - Edit tracker.

Arguments:

```json
[
    {
        "type": "File",
        "name": "type",
        "description": "Empty"
    },
    {
        "type": "File",
        "name": "campaign_id",
        "description": "Empty"
    },
    {
        "type": "Text",
        "name": "name",
        "description": "Enter tracker name"
    },
    {
        "type": "File",
        "name": "settings",
        "description": "Empty"
    },
    {
        "type": "Select",
        "name": "creator_id",
        "description": "Choose affiliate"
    },
    {
        "type": "Text",
        "name": "fire",
        "description": "Fire URL"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[type]=something

- attributes[campaign_id]=something

- attributes[name]=something

- attributes[settings]=something

- attributes[creator_id]=something

- attributes[fire]=something




+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + type: `-` (required, string) - Empty
        + campaign_id: `-` (required, string) - Empty
        + name: `-` (required, string) - Enter tracker name
        + settings: `-` (required, string) - Empty
        + creator_id: `-` (required, string) - Choose affiliate
        + fire: `-` (required, string) - Fire URL  
          


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }


## History Actions [/api/v6/terms/History/]

### EditDescription [GET /api/v6/action/History/EditDescription/execute/1{?token,perPage,page}]

Action from History namespace, short description - Edit Communication.

Arguments:

```json
[
    {
        "type": "TextArea",
        "name": "description",
        "description": "Edit description"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[description]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + description: `-` (required, string) - Edit description  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }


## Communication Actions [/api/v6/terms/Communication/]

### Edit [GET /api/v6/action/Communication/Edit/execute/1{?token,perPage,page}]

Action from Communication namespace, short description - Edit Communication.

Arguments:

```json
[
    {
        "type": "Text",
        "name": "title",
        "description": "Title"
    },
    {
        "type": "Text",
        "name": "description",
        "description": "Description"
    },
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[title]=something
- attributes[description]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + title: `-` (required, string) - Title  
        + description: `-` (required, string) - Description


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### EditImportant [GET /api/v6/action/Communication/EditImportant/execute/1{?token,perPage,page}]

Action from Communication namespace, short description - Edit State Important Communication.

Arguments:

```json
[
    {
        "type": "Select",
        "name": "state_important",
        "description": "Choose state important"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[state_important]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + state_important: `-` (required, string) - Choose state important  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }


## Transaction Actions [/api/v6/terms/Transaction/]

### AddBeneficiary [GET /api/v6/action/Transaction/AddBeneficiary/execute/1{?token,perPage,page}]

Action from Transaction namespace, short description - Add Beneficiary.

Arguments:

```json
[
    {
        "type": "Select",
        "name": "employee_id",
        "description": "Add Beneficiary"
    },
    {
        "type": "Number",
        "name": "percentage",
        "description": "Percentage amount"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[employee_id]=something

- attributes[percentage]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + employee_id: `-` (required, string) - Add Beneficiary
        + percentage: `-` (required, string) - Percentage amount  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }


## Group Actions [/api/v6/terms/Group/]

### AssignCustomer [GET /api/v6/action/Group/AssignCustomer/execute/1{?token,perPage,page}]

Action from Group namespace, short description - Assign customer to group.

Arguments:

```json
[
    {
        "type": "Autocomplete",
        "name": "customer",
        "description": "Choose customer"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[customer]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + customer: `-` (required, string) - Choose customer  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### CreateNew [GET /api/v6/action/Group/CreateNew/execute/1{?token,perPage,page}]

Action from Group namespace, short description - Create new group.

Arguments:

```json
[
    {
        "type": "Text",
        "name": "name",
        "description": "Enter your new group name"
    },
    {
        "type": "Text",
        "name": "bm_trader_group_id",
        "description": "Enter BM trader group ID"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[name]=something

- attributes[bm_trader_group_id]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + name: `-` (required, string) - Enter your new group name
        + bm_trader_group_id: `-` (required, string) - Enter BM trader group ID  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### DetachCustomer [GET /api/v6/action/Group/DetachCustomer/execute/1{?token,perPage,page}]

Action from Group namespace, short description - Detach customer from group.

Arguments:

```json
[
    {
        "type": "Autocomplete",
        "name": "customer_id",
        "description": "Select customer"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[customer_id]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + customer_id: `-` (required, string) - Select customer  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### Edit [GET /api/v6/action/Group/Edit/execute/1{?token,perPage,page}]

Action from Group namespace, short description - Edit group.

Arguments:

```json
[
    {
        "type": "Text",
        "name": "name",
        "description": "Enter your new group name"
    },
    {
        "type": "Text",
        "name": "bm_trader_group_id",
        "description": "Enter BM trader group ID"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[name]=something

- attributes[bm_trader_group_id]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + name: `-` (required, string) - Enter your new group name
        + bm_trader_group_id: `-` (required, string) - Enter BM trader group ID  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### EditBMTraderGroupID [GET /api/v6/action/Group/EditBMTraderGroupID/execute/1{?token,perPage,page}]

Action from Group namespace, short description - Edit BM trader group ID.

Arguments:

```json
[
    {
        "type": "Text",
        "name": "name",
        "description": "Enter name"
    },
    {
        "type": "Text",
        "name": "bm_trader_group_id",
        "description": "Enter BM trader group ID"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[name]=something
- attributes[bm_trader_group_id]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + name: `-` (required, string) - Enter name
        + bm_trader_group_id: `-` (required, string) - Enter BM trader group ID  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### EditName [GET /api/v6/action/Group/EditName/execute/1{?token,perPage,page}]

Action from Group namespace, short description - Edit name to group.

Arguments:

```json
[
    {
        "type": "Text",
        "name": "name",
        "description": "Enter your new group name"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[name]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + name: `-` (required, string) - Enter your new group name  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }


## ShiftManagement Actions [/api/v6/terms/ShiftManagement/]

### CreateNew [GET /api/v6/action/ShiftManagement/CreateNew/execute/1{?token,perPage,page}]

Action from ShiftManagement namespace, short description - Create new group.

Arguments:

```json
[
    {
        "type": "Text",
        "name": "name",
        "description": "Enter your new shift name"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[name]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + name: `-` (required, string) - Enter your new shift name  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### EditName [GET /api/v6/action/ShiftManagement/EditName/execute/1{?token,perPage,page}]

Action from ShiftManagement namespace, short description - Edit name to shift management.

Arguments:

```json
[
    {
        "type": "Text",
        "name": "name",
        "description": "Enter your new shift name"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[name]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + name: `-` (required, string) - Enter your new shift name  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### AssignEmployee [GET /api/v6/action/ShiftManagement/AssignEmployee/execute/1{?token,perPage,page}]

Action from ShiftManagement namespace, short description - Assign customer to shift management.

Arguments:

```json
[
    {
        "type": "Select",
        "name": "employee_id",
        "description": "Choose broker"
    },
    {
        "type": "File",
        "name": "shift_id",
        "description": "Empty"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[employee_id]=something

- attributes[shift_id]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + employee_id: `-` (required, string) - Choose broker
        + shift_id: `-` (required, string) - Empty  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### DetachEmployee [GET /api/v6/action/ShiftManagement/DetachEmployee/execute/1{?token,perPage,page}]

Action from ShiftManagement namespace, short description - Detach customer from group.

Arguments:

```json
[
    {
        "type": "Select",
        "name": "employee_id",
        "description": "Choice worker that will be detached from desk"
    },
    {
        "type": "File",
        "name": "shift_id",
        "description": "Empty"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[employee_id]=something

- attributes[shift_id]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + employee_id: `-` (required, string) - Choice worker that will be detached from desk
        + shift_id: `-` (required, string) - Empty  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### Edit [GET /api/v6/action/ShiftManagement/Edit/execute/1{?token,perPage,page}]

Action from ShiftManagement namespace, short description - Edit group.

Arguments:

```json
[
    {
        "type": "Text",
        "name": "name",
        "description": "Enter your new shift name"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[name]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + name: `-` (required, string) - Enter your new shift name  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }


## Remark Actions [/api/v6/terms/Remark/]

### DeleteRemark [GET /api/v6/action/Remark/DeleteRemark/execute/1{?token,perPage,page}]

Action from Remark namespace, short description - Delete remark.

Arguments:

```json
[]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:




+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
          


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }


## Notification Actions [/api/v6/terms/Notification/]

### CreateNewEmail [GET /api/v6/action/Notification/CreateNewEmail/execute/1{?token,perPage,page}]

Action from Notification namespace, short description - Create new email notification.

Arguments:

```json
[
    {
        "type": "File",
        "name": "method",
        "description": "Empty"
    },
    {
        "type": "Select",
        "name": "type",
        "description": "Choice type from list"
    },
    {
        "type": "Select",
        "name": "email_template_id",
        "description": "Choice emil template from list"
    },
    {
        "type": "Text",
        "name": "to",
        "description": "Enter email address"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[method]=something

- attributes[type]=something

- attributes[email_template_id]=something

- attributes[to]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + method: `-` (required, string) - Empty
        + type: `-` (required, string) - Choice type from list
        + email_template_id: `-` (required, string) - Choice emil template from list
        + to: `-` (required, string) - Enter email address  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### EditMailTemplate [GET /api/v6/action/Notification/EditMailTemplate/execute/1{?token,perPage,page}]

Action from Notification namespace, short description - Edit mail template setting notification.

Arguments:

```json
[
    {
        "type": "Select",
        "name": "email_template_id",
        "description": "Choice emil template from list"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[email_template_id]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + email_template_id: `-` (required, string) - Choice emil template from list  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### EditMethod [GET /api/v6/action/Notification/EditMethod/execute/1{?token,perPage,page}]

Action from Notification namespace, short description - Edit method notification.

Arguments:

```json
[
    {
        "type": "File",
        "name": "method",
        "description": "Empty"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[method]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + method: `-` (required, string) - Empty  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### EditToEmail [GET /api/v6/action/Notification/EditToEmail/execute/1{?token,perPage,page}]

Action from Notification namespace, short description - Edit recipient setting notification.

Arguments:

```json
[
    {
        "type": "Text",
        "name": "to",
        "description": "Enter email address"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[to]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + to: `-` (required, string) - Enter email address  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### EditType [GET /api/v6/action/Notification/EditType/execute/1{?token,perPage,page}]

Action from Notification namespace, short description - Edit type notification.

Arguments:

```json
[
    {
        "type": "Select",
        "name": "type",
        "description": "Choice type from list"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[type]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + type: `-` (required, string) - Choice type from list  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }


## Ticket Actions [/api/v6/terms/Ticket/]

### ChangeBroker [POST /api/v6/action/Ticket/ChangeBroker/execute/1{?token,perPage,page}]

Action from Ticket namespace, short description - Change broker ticket.

Arguments:

```json
[
    {
        "type": "Select",
        "name": "employee_id",
        "description": "Choice broker from list"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[employee_id]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + employee_id: `-` (required, string) - Choice broker from list  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### ChangeCreatedAt [POST /api/v6/action/Ticket/ChangeCreatedAt/execute/1{?token,perPage,page}]

Action from Ticket namespace, short description - Change created at ticket.

Arguments:

```json
[
    {
        "type": "DateTime",
        "name": "created_at",
        "description": "Created at"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[created_at]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + created_at: `-` (required, string) - Created at  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### ChangeAmount [GET /api/v6/action/Ticket/ChangeAmount/execute/1{?token,perPage,page}]

Action from Ticket namespace, short description - Change amount at ticket.

Arguments:

```json
[
    {
        "type": "Number",
        "name": "amountwithdrawal",
        "description": "Amount"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[amountwithdrawal]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + amountwithdrawal: `-` (required, string) - Amount  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### WithdrawalApprove [GET /api/v6/action/Ticket/WithdrawalApprove/execute/1{?token,perPage,page}]

Action from Ticket namespace, short description - Approve withdrawal ticket.

Arguments:

```json
[
    {
        "type": "Select",
        "name": "method",
        "description": "Select type of withdrawal"
    },
    {
        "type": "Text",
        "name": "description",
        "description": "A reason for withdrawal"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[method]=something

- attributes[description]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + method: `-` (required, string) - Select type of withdrawal
        + description: `-` (required, string) - A reason for withdrawal  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### Decline [GET /api/v6/action/Ticket/Decline/execute/1{?token,perPage,page}]

Action from Ticket namespace, short description - Decline ticket.

Arguments:

```json
[
    {
        "type": "Text",
        "name": "decline_title",
        "description": "Enter a short decline-message title"
    },
    {
        "type": "TextArea",
        "name": "decline_message",
        "description": "Enter reason for decline-message ticket"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[decline_title]=something

- attributes[decline_message]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + decline_title: `-` (required, string) - Enter a short decline-message title
        + decline_message: `-` (required, string) - Enter reason for decline-message ticket  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### DepositApprove [GET /api/v6/action/Ticket/DepositApprove/execute/1{?token,perPage,page}]

Action from Ticket namespace, short description - Approve ticket.

Arguments:

```json
[]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:




+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
          


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### EditDeclineMessage [GET /api/v6/action/Ticket/EditDeclineMessage/execute/1{?token,perPage,page}]

Action from Ticket namespace, short description - Edit decline message.

Arguments:

```json
[
    {
        "type": "Text",
        "name": "decline_title",
        "description": "Enter a short decline-message title"
    },
    {
        "type": "TextArea",
        "name": "decline_message",
        "description": "Enter reason for decline-message ticket"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[decline_title]=something

- attributes[decline_message]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + decline_title: `-` (required, string) - Enter a short decline-message title
        + decline_message: `-` (required, string) - Enter reason for decline-message ticket  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }


## Desk Actions [/api/v6/terms/Desk/]

### Activate [GET /api/v6/action/Desk/Activate/execute/1{?token,perPage,page}]

Action from Desk namespace, short description - Activate desk.

Arguments:

```json
[]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:




+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
          


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### AssignCustomer [GET /api/v6/action/Desk/AssignCustomer/execute/1{?token,perPage,page}]

Action from Desk namespace, short description - Attach trader to desk.

Arguments:

```json
[
    {
        "type": "Autocomplete",
        "name": "customer_id",
        "description": "Select trader"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[customer_id]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + customer_id: `-` (required, string) - Select trader  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### AssignWorker [GET /api/v6/action/Desk/AssignWorker/execute/1{?token,perPage,page}]

Action from Desk namespace, short description - Attach worker to desk.

Arguments:

```json
[
    {
        "type": "Select",
        "name": "employee_id",
        "description": "Choose broker"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[employee_id]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + employee_id: `-` (required, string) - Choose broker  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### CreateNew [GET /api/v6/action/Desk/CreateNew/execute/1{?token,perPage,page}]

Action from Desk namespace, short description - Create new desk.

Arguments:

```json
[
    {
        "type": "Text",
        "name": "name",
        "description": "Enter your new desk name"
    },
    {
        "type": "MultiSelect",
        "name": "country",
        "description": "Choice country from list"
    },
    {
        "type": "MultiSelect",
        "name": "language",
        "description": "Choice language from list"
    },
    {
        "type": "Select",
        "name": "parent_id",
        "description": "Choice parent from list"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[name]=something

- attributes[country]=something

- attributes[language]=something

- attributes[parent_id]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + name: `-` (required, string) - Enter your new desk name
        + country: `-` (required, string) - Choice country from list
        + language: `-` (required, string) - Choice language from list
        + parent_id: `-` (required, string) - Choice parent from list  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### Deactivate [GET /api/v6/action/Desk/Deactivate/execute/1{?token,perPage,page}]

Action from Desk namespace, short description - Deactivate desk.

Arguments:

```json
[]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:




+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
          


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### DetachCustomer [GET /api/v6/action/Desk/DetachCustomer/execute/1{?token,perPage,page}]

Action from Desk namespace, short description - Detach trader from desk.

Arguments:

```json
[
    {
        "type": "Autocomplete",
        "name": "customer_id",
        "description": "Choice trader that will be detached from desk"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[customer_id]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + customer_id: `-` (required, string) - Choice trader that will be detached from desk  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### DetachWorker [GET /api/v6/action/Desk/DetachWorker/execute/1{?token,perPage,page}]

Action from Desk namespace, short description - Detach worker from desk.

Arguments:

```json
[
    {
        "type": "Select",
        "name": "employee_id",
        "description": "Choice worker that will be detached from desk"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[employee_id]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + employee_id: `-` (required, string) - Choice worker that will be detached from desk  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### DisableSplitter [GET /api/v6/action/Desk/DisableSplitter/execute/1{?token,perPage,page}]

Action from Desk namespace, short description - Disable lead splitter and make desk active.

Arguments:

```json
[]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:




+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
          


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### Edit [GET /api/v6/action/Desk/Edit/execute/1{?token,perPage,page}]

Action from Desk namespace, short description - Edit desk.

Arguments:

```json
[
    {
        "type": "Text",
        "name": "name",
        "description": "Enter your new desk name"
    },
    {
        "type": "MultiSelect",
        "name": "country",
        "description": "Choice country from list"
    },
    {
        "type": "MultiSelect",
        "name": "language",
        "description": "Choice language from list"
    },
    {
        "type": "Select",
        "name": "parent_id",
        "description": "Choice parent from list"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[name]=something

- attributes[country]=something

- attributes[language]=something

- attributes[parent_id]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + name: `-` (required, string) - Enter your new desk name
        + country: `-` (required, string) - Choice country from list
        + language: `-` (required, string) - Choice language from list
        + parent_id: `-` (required, string) - Choice parent from list  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### EditCountry [GET /api/v6/action/Desk/EditCountry/execute/1{?token,perPage,page}]

Action from Desk namespace, short description - Edit country to desk.

Arguments:

```json
[
    {
        "type": "MultiSelect",
        "name": "country",
        "description": "Choice country from list"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[country]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + country: `-` (required, string) - Choice country from list  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### EditLanguage [GET /api/v6/action/Desk/EditLanguage/execute/1{?token,perPage,page}]

Action from Desk namespace, short description - Edit language to desk.

Arguments:

```json
[
    {
        "type": "MultiSelect",
        "name": "language",
        "description": "Choice language from list"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[language]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + language: `-` (required, string) - Choice language from list  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### EditName [GET /api/v6/action/Desk/EditName/execute/1{?token,perPage,page}]

Action from Desk namespace, short description - Edit name to desk.

Arguments:

```json
[
    {
        "type": "Text",
        "name": "name",
        "description": "Enter your new desk name"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[name]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + name: `-` (required, string) - Enter your new desk name  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### EditParent [GET /api/v6/action/Desk/EditParent/execute/1{?token,perPage,page}]

Action from Desk namespace, short description - Edit parent to desk.

Arguments:

```json
[
    {
        "type": "Select",
        "name": "parent_id",
        "description": "Choice parent from list"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[parent_id]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + parent_id: `-` (required, string) - Choice parent from list  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### Remove [GET /api/v6/action/Desk/Remove/execute/1{?token,perPage,page}]

Action from Desk namespace, short description - Remove desk.

Arguments:

```json
[]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:




+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
          


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }


## Employee Actions [/api/v6/terms/Employee/]

### BlockLogin [GET /api/v6/action/Employee/BlockLogin/execute/1{?token,perPage,page}]

Action from Employee namespace, short description - Block worker login.

Arguments:

```json
[]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:




+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
          


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### UnblockLogin [GET /api/v6/action/Employee/UnblockLogin/execute/1{?token,perPage,page}]

Action from Employee namespace, short description - Unblock worker login.

Arguments:

```json
[]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:




+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
          


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### ChangePassword [GET /api/v6/action/Employee/ChangePassword/execute/1{?token,perPage,page}]

Action from Employee namespace, short description - Change password.

Arguments:

```json
[
    {
        "type": "Password",
        "name": "password",
        "description": "Worker password"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[password]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + password: `-` (required, string) - Worker password  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### CreateNew [GET /api/v6/action/Employee/CreateNew/execute/1{?token,perPage,page}]

Action from Employee namespace, short description - Create new worker.

Arguments:

```json
[
    {
        "type": "Text",
        "name": "login",
        "description": "Enter your worker login"
    },
    {
        "type": "Password",
        "name": "password",
        "description": "Worker password"
    },
    {
        "type": "Text",
        "name": "fname",
        "description": "Enter your new worker first name"
    },
    {
        "type": "Text",
        "name": "lname",
        "description": "Enter your new worker last name"
    },
    {
        "type": "Select",
        "name": "language",
        "description": "Choice language from list"
    },
    {
        "type": "Select",
        "name": "group",
        "description": "Choice group from list"
    },
    {
        "type": "MultiSelect",
        "name": "desk_id",
        "description": "Choice desk from list"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[login]=something

- attributes[password]=something

- attributes[fname]=something

- attributes[lname]=something

- attributes[language]=something

- attributes[group]=something

- attributes[desk_id]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + login: `-` (required, string) - Enter your worker login
        + password: `-` (required, string) - Worker password
        + fname: `-` (required, string) - Enter your new worker first name
        + lname: `-` (required, string) - Enter your new worker last name
        + language: `-` (required, string) - Choice language from list
        + group: `-` (required, string) - Choice group from list
        + desk_id: `-` (required, string) - Choice desk from list  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### Edit [GET /api/v6/action/Employee/Edit/execute/1{?token,perPage,page}]

Action from Employee namespace, short description - Edit worker.

Arguments:

```json
[
    {
        "type": "Text",
        "name": "fname",
        "description": "Enter your new worker first name"
    },
    {
        "type": "Text",
        "name": "lname",
        "description": "Enter your new worker last name"
    },
    {
        "type": "Text",
        "name": "phone",
        "description": "Enter your new worker phone"
    },
    {
        "type": "Text",
        "name": "email",
        "description": "Enter your new worker email"
    },
    {
        "type": "Select",
        "name": "country",
        "description": "Choice country from list"
    },
    {
        "type": "Select",
        "name": "language",
        "description": "Choice language from list"
    },
    {
        "type": "Select",
        "name": "group",
        "description": "Choice group from list"
    },
    {
        "type": "Select",
        "name": "account_id",
        "description": "Choice email account from list"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[fname]=something

- attributes[lname]=something

- attributes[phone]=something

- attributes[email]=something

- attributes[country]=something

- attributes[language]=something

- attributes[group]=something

- attributes[account_id]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + fname: `-` (required, string) - Enter your new worker first name
        + lname: `-` (required, string) - Enter your new worker last name
        + phone: `-` (required, string) - Enter your new worker phone
        + email: `-` (required, string) - Enter your new worker email
        + country: `-` (required, string) - Choice country from list
        + language: `-` (required, string) - Choice language from list
        + group: `-` (required, string) - Choice group from list
        + account_id: `-` (required, string) - Choice email account from list  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### EditCountry [GET /api/v6/action/Employee/EditCountry/execute/1{?token,perPage,page}]

Action from Employee namespace, short description - Edit worker country.

Arguments:

```json
[
    {
        "type": "Select",
        "name": "country",
        "description": "Choice country from list"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[country]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + country: `-` (required, string) - Choice country from list  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### EditEmail [GET /api/v6/action/Employee/EditEmail/execute/1{?token,perPage,page}]

Action from Employee namespace, short description - Edit worker email.

Arguments:

```json
[
    {
        "type": "Text",
        "name": "email",
        "description": "Enter your new worker email"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[email]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + email: `-` (required, string) - Enter your new worker email  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### EditFName [GET /api/v6/action/Employee/EditFName/execute/1{?token,perPage,page}]

Action from Employee namespace, short description - Edit worker first name.

Arguments:

```json
[
    {
        "type": "Text",
        "name": "fname",
        "description": "Enter your new worker first name"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[fname]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + fname: `-` (required, string) - Enter your new worker first name  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### EditLName [GET /api/v6/action/Employee/EditLName/execute/1{?token,perPage,page}]

Action from Employee namespace, short description - Edit worker last name.

Arguments:

```json
[
    {
        "type": "Text",
        "name": "lname",
        "description": "Enter your new worker last name"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[lname]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + lname: `-` (required, string) - Enter your new worker last name  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### EditGroup [GET /api/v6/action/Employee/EditGroup/execute/1{?token,perPage,page}]

Action from Employee namespace, short description - Edit worker department.

Arguments:

```json
[
    {
        "type": "Select",
        "name": "group",
        "description": "Choice group from list"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[group]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + group: `-` (required, string) - Choice group from list  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### EditLanguage [GET /api/v6/action/Employee/EditLanguage/execute/1{?token,perPage,page}]

Action from Employee namespace, short description - Edit worker language.

Arguments:

```json
[
    {
        "type": "Select",
        "name": "language",
        "description": "Choice language from list"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[language]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + language: `-` (required, string) - Choice language from list  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### EditLogin [GET /api/v6/action/Employee/EditLogin/execute/1{?token,perPage,page}]

Action from Employee namespace, short description - Edit worker login.

Arguments:

```json
[
    {
        "type": "Text",
        "name": "login",
        "description": "Enter your new worker login"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[login]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + login: `-` (required, string) - Enter your new worker login  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### EditPhone [GET /api/v6/action/Employee/EditPhone/execute/1{?token,perPage,page}]

Action from Employee namespace, short description - Edit worker phone.

Arguments:

```json
[
    {
        "type": "Text",
        "name": "phone",
        "description": "Enter your new worker phone"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[phone]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + phone: `-` (required, string) - Enter your new worker phone  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### EditVoiceSpinAgent [GET /api/v6/action/Employee/EditVoiceSpinAgent/execute/1{?token,perPage,page}]

Action from Employee namespace, short description - Edit worker dialer agent.

Arguments:

```json
[
    {
        "type": "Text",
        "name": "voicespin_agent",
        "description": "Enter your new agent field"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[voicespin_agent]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + voicespin_agent: `-` (required, string) - Enter your new agent field  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### EditVoiceSpinExtension [GET /api/v6/action/Employee/EditVoiceSpinExtension/execute/1{?token,perPage,page}]

Action from Employee namespace, short description - Edit worker dialer extension.

Arguments:

```json
[
    {
        "type": "Text",
        "name": "voicespin_extension",
        "description": "Enter your new agent field"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[voicespin_extension]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + voicespin_extension: `-` (required, string) - Enter your new agent field  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### Notify [GET /api/v6/action/Employee/Notify/execute/1{?token,perPage,page}]

Action from Employee namespace, short description - Send notify to worker.

Arguments:

```json
[
    {
        "type": "Text",
        "name": "message",
        "description": "Enter your message"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[message]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + message: `-` (required, string) - Enter your message  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

### EditShift [GET /api/v6/action/Employee/EditShift/execute/1{?token,perPage,page}]

Action from Employee namespace, short description - Edit worker shift.

Arguments:

```json
[
    {
        "type": "Select",
        "name": "shift_id",
        "description": "Choice shift from list"
    }
]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:

- attributes[shift_id]=something


+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
        + shift_id: `-` (required, string) - Choice shift from list  


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }


## SmsTemplate Actions [/api/v6/terms/SmsTemplate/]

### Remove [GET /api/v6/action/SmsTemplate/Remove/execute/1{?token,perPage,page}]

Action from SmsTemplate namespace, short description - Remove template.

Arguments:

```json
[]
```

**NOTE:** Data should be represented as attributes[name], instead of raw json

For example like this:




+ Parameters
    + token: `YOUR_TOKEN_HERE` (required, text) ... Your secret token for auth
    

+ Request (application/json)

    + Attributes
          


+ Response 200 (application/json)

        {
          "data": [
            {
                "something" : "something"
            }
        }

