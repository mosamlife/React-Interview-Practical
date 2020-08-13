# React_exercise

# Sort array in ascending order 

* Without Using Array method to sort
* response time doesn't matter in logic
* array = 4,2,4,3,1,5
* array = 0, 1, 2, 4, 8,5,8, 4, 2, 1, 0


# Sort comments
* reply_id refers to comment id
* null reply_id means primary comments
--------
### input
~~~~
[
    {
        "id": 1,
        "post_id": 1,
        "user_id": 1,
        "comments": "Hello",
        "reply_id": null,
        "createdAt": "2019-09-04T08:40:34.000Z",
        "updatedAt": "2019-09-04T08:40:34.000Z"
    },
    {
        "id": 2,
        "post_id": 1,
        "user_id": 1,
        "comments": "Hii",
        "reply_id": 1,
        "createdAt": "2019-09-04T08:40:34.000Z",
        "updatedAt": "2019-09-04T08:40:34.000Z"
    },
    {
        "id": 3,
        "post_id": 1,
        "user_id": 1,
        "comments": "Hey",
        "reply_id": 1,
        "createdAt": "2019-09-04T08:40:34.000Z",
        "updatedAt": "2019-09-04T08:40:34.000Z"
    },
    {
        "id": 4,
        "post_id": 1,
        "user_id": 1,
        "comments": "Hey2",
        "reply_id": 3,
        "createdAt": "2019-09-04T08:40:34.000Z",
        "updatedAt": "2019-09-04T08:40:34.000Z"
    },
    {
        "id": 5,
        "post_id": 1,
        "user_id": 1,
        "comments": "OK",
        "reply_id": 2,
        "createdAt": "2019-09-04T08:40:34.000Z",
        "updatedAt": "2019-09-04T08:40:34.000Z"
    },
    {
        "id": 6,
        "post_id": 1,
        "user_id": 1,
        "comments": "Hh",
        "reply_id": null,
        "createdAt": "2019-09-04T08:40:34.000Z",
        "updatedAt": "2019-09-04T08:40:34.000Z"
    },
    {
        "id": 7,
        "post_id": 1,
        "user_id": 1,
        "comments": "Hee",
        "reply_id": 6,
        "createdAt": "2019-09-04T08:40:34.000Z",
        "updatedAt": "2019-09-04T08:40:34.000Z"
    },
    {
        "id": 8,
        "post_id": 1,
        "user_id": 1,
        "comments": "Hii",
        "reply_id": 4,
        "createdAt": "2019-09-04T08:40:34.000Z",
        "updatedAt": "2019-09-04T08:40:34.000Z"
    },
]
~~~~
------------
### output
~~~~
{
    "comments": {
        "1": {
            "post_id": 1,
            "user_id": 1,
            "comments": "Hello",
            "replies": {
                "2": {
                    "post_id": 1,
                    "user_id": 1,
                    "comments": "Hii",
                    "replies": {
                        "5": {
                            "post_id": 1,
                            "user_id": 1,
                            "comments": "OK",
                            "replies": {}
                        }
                    }
                },
                "3": {
                    "post_id": 1,
                    "user_id": 1,
                    "comments": "Hey",
                    "replies": {
                        "4": {
                            "post_id": 1,
                            "user_id": 1,
                            "comments": "Hey2",
                            "replies": {
                                "8": {
                                    "post_id": 1,
                                    "user_id": 1,
                                    "comments": "Hii",
                                    "replies": {}
                                }
                            }
                        }
                    }
                }
            }
        },
        "6": {
            "post_id": 1,
            "user_id": 1,
            "comments": "Hh",
            "replies": {
                "7": {
                    "post_id": 1,
                    "user_id": 1,
                    "comments": "Hee",
                    "replies": {}
                }
            }
        }
    }
}
~~~~

------------
 ### Display this object in Table 
~~~~

  {
    "medications":[{
            "aceInhibitors":[{
                "name":"lisinopril",
                "strength":"10 mg Tab",
                "dose":"1 tab",
                "route":"PO",
                "sig":"daily",
                "pillCount":"#90",
                "refills":"Refill 3"
            }],
            "antianginal":[{
                "name":"nitroglycerin",
                "strength":"0.4 mg Sublingual Tab",
                "dose":"1 tab",
                "route":"SL",
                "sig":"q15min PRN",
                "pillCount":"#30",
                "refills":"Refill 1"
            }],
            "anticoagulants":[{
                "name":"warfarin sodium",
                "strength":"3 mg Tab",
                "dose":"1 tab",
                "route":"PO",
                "sig":"daily",
                "pillCount":"#90",
                "refills":"Refill 3"
            }],
            "betaBlocker":[{
                "name":"metoprolol tartrate",
                "strength":"25 mg Tab",
                "dose":"1 tab",
                "route":"PO",
                "sig":"daily",
                "pillCount":"#90",
                "refills":"Refill 3"
            }],
            "diuretic":[{
                "name":"furosemide",
                "strength":"40 mg Tab",
                "dose":"1 tab",
                "route":"PO",
                "sig":"daily",
                "pillCount":"#90",
                "refills":"Refill 3"
            }],
            "mineral":[{
                "name":"potassium chloride ER",
                "strength":"10 mEq Tab",
                "dose":"1 tab",
                "route":"PO",
                "sig":"daily",
                "pillCount":"#90",
                "refills":"Refill 3"
            }]
        }
    ],
    "labs":[{
        "name":"Arterial Blood Gas",
        "time":"Today",
        "location":"Main Hospital Lab"      
        },
        {
        "name":"BMP",
        "time":"Today",
        "location":"Primary Care Clinic"    
        },
        {
        "name":"BNP",
        "time":"3 Weeks",
        "location":"Primary Care Clinic"    
        },
        {
        "name":"BUN",
        "time":"1 Year",
        "location":"Primary Care Clinic"    
        },
        {
        "name":"Cardiac Enzymes",
        "time":"Today",
        "location":"Primary Care Clinic"    
        },
        {
        "name":"CBC",
        "time":"1 Year",
        "location":"Primary Care Clinic"    
        },
        {
        "name":"Creatinine",
        "time":"1 Year",
        "location":"Main Hospital Lab"  
        },
        {
        "name":"Electrolyte Panel",
        "time":"1 Year",
        "location":"Primary Care Clinic"    
        },
        {
        "name":"Glucose",
        "time":"1 Year",
        "location":"Main Hospital Lab"  
        },
        {
        "name":"PT/INR",
        "time":"3 Weeks",
        "location":"Primary Care Clinic"    
        },
        {
        "name":"PTT",
        "time":"3 Weeks",
        "location":"Coumadin Clinic"    
        },
        {
        "name":"TSH",
        "time":"1 Year",
        "location":"Primary Care Clinic"    
        }
    ],
    "imaging":[{
        "name":"Chest X-Ray",
        "time":"Today",
        "location":"Main Hospital Radiology"    
        },
        {
        "name":"Chest X-Ray",
        "time":"Today",
        "location":"Main Hospital Radiology"    
        },
        {
        "name":"Chest X-Ray",
        "time":"Today",
        "location":"Main Hospital Radiology"    
        }
    ]
}


~~~~

## Which method do you prefer to clone an array, and why?
* one: [...arr];
* two: arr.slice(0);
* three: Array.from(arr);
* four: arr.map((x) => x);
* five: arr.concat([]);
* six: JSON.parse(JSON.stringify(arr));

## Which method do you prefer to flatten an array & why?
* one: arr.flat();
* two: [].concat(...arr);
* three: arr.reduce((acc, val) => acc.concat(val), []);
    
## Implement Dark and White mode in React 
* Without Using Library

## Which is Possibly the easiest way to create an array with unique elements in it

values = 😀	😁	🤪 😀 😁


