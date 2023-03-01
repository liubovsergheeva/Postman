HW_1 Postman
	
	
ключи надо заполнить
вместо str - слово , вместо int цифры	
Создать запросы в Postman. 

Protocol: http
IP: 162.55.220.72
Port: 5005

EP_1
Method: GET
EndPoint: /get_method
request url params: 
 name: str
 age: int

response: 
[
    “Str”,
    “Str”
]	http://162.55.220.72:5005/get_method?name=str&age=int

[
    "LiubovSergeeva",
    "18"
]

EP_2
Method: POST
EndPoint: /user_info_3
request form data: 
 name: str
 age: int
 salary: int

response: 
{'name': name,
          'age': age,
          'salary': salary,
          'family': {'children': [['Alex', 24], ['Kate', 12]],
                     'u_salary_1_5_year': salary * 4}}	http://162.55.220.72:5005/user_info_3?name=str&age=int&salary=int

{
    "age": "18",
    "family": {
        "children": [
            [
                "Alex",
                24
            ],
            [
                "Kate",
                12
            ]
        ],
        "u_salary_1_5_year": 40000
    },
    "name": "LiubovSergeeva",
    "salary": 10000
}

EP_3
Method: GET
EndPoint: /object_info_1
request url params: 
 name: str
 age: int
 weight: int

response: 
{'name': name,
          'age': age,
          'daily_food': weight * 0.012,
          'daily_sleep': weight * 2.5}	http://162.55.220.72:5005/object_info_1?name=str&age=int&weight=int

{
    "age": 18,
    "daily_food": 0.72,
    "daily_sleep": 150.0,
    "name": "LiubovSergeeva"
}

EP_4
Method: GET
EndPoint: /object_info_2
request url params: 
 name: str
 age: int
 salary: int

response: 
{'start_qa_salary': salary,
          'qa_salary_after_6_months': salary * 2,
          'qa_salary_after_12_months': salary * 2.7,
          'qa_salary_after_1.5_year': salary * 3.3,
          'qa_salary_after_3.5_years': salary * 3.8,
          'person': {'u_name': [user_name, salary, age],
                     'u_age': age,
                     'u_salary_5_years': salary * 4.2}
          }	http://162.55.220.72:5005/object_info_2?name=str&age=int&salary=int

{
    "person": {
        "u_age": 18,
        "u_name": [
            "LiubovSergeeva",
            10000,
            18
        ],
        "u_salary_5_years": 42000.0
    },
    "qa_salary_after_1.5_year": 33000.0,
    "qa_salary_after_12_months": 27000.0,
    "qa_salary_after_3.5_years": 38000.0,
    "qa_salary_after_6_months": 20000,
    "start_qa_salary": 10000
}

EP_5
Method: GET
EndPoint: /object_info_3
request url params: 
 name: str
 age: int
 salary: int

response: 
{'name': name,
          'age': age,
          'salary': salary,
          'family': {'children': [['Alex', 24], ['Kate', 12]],
                     'pets': {'cat':{'name':'Sunny',
                                     'age': 3},
                              'dog':{'name':'Luky',
                                     'age': 4}},
                     'u_salary_1_5_year': salary * 4}
          }	http://162.55.220.72:5005/object_info_3?name=str&age=int&salary=int
{
    "age": "18",
    "family": {
        "children": [
            [
                "Alex",
                24
            ],
            [
                "Kate",
                12
            ]
        ],
        "pets": {
            "cat": {
                "age": 3,
                "name": "Sunny"
            },
            "dog": {
                "age": 4,
                "name": "Luky"
            }
        },
        "u_salary_1_5_year": 40000
    },
    "name": "LiubovSergeeva",
    "salary": 10000
}

EP_6
Method: GET
EndPoint: /object_info_4
request url params: 
 name: str
 age: int
 salary: int

response: 
{'name': name,
          'age': int(age),
          'salary': [salary, str(salary * 2), str(salary * 3)]}	http://162.55.220.72:5005/object_info_4?name=str&age=int&salary=int
{
    "age": 18,
    "name": "LiubovSergeeva",
    "salary": [
        10000,
        "20000",
        "30000"
    ]
}

EP_7
Method: POST
EndPoint: /user_info_2
request form data: 
 name: str
 age: int
 salary: int

response: 
{'start_qa_salary': salary,
          'qa_salary_after_6_months': salary * 2,
          'qa_salary_after_12_months': salary * 2.7,
          'qa_salary_after_1.5_year': salary * 3.3,
          'qa_salary_after_3.5_years': salary * 3.8,
          'person': {'u_name': [user_name, salary, age],
                     'u_age': age,
                     'u_salary_5_years': salary * 4.2}
          }	http://162.55.220.72:5005/user_info_2?name=str&age=int&salary=int
{
    "person": {
        "u_age": 18,
        "u_name": [
            "LiubovSergeeva",
            10000,
            18
        ],
        "u_salary_5_years": 42000.0
    },
    "qa_salary_after_1.5_year": 33000.0,
    "qa_salary_after_12_months": 27000.0,
    "qa_salary_after_3.5_years": 38000.0,
    "qa_salary_after_6_months": 20000,
    "start_qa_salary": 10000
}

	
