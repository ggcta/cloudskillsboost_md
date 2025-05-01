---
id: 690
name: 'Google Security Operations - SIEM Rules'
type: Course
url: https://www.cloudskillsboost.google/course_templates/690
date_published: 2024-05-07
topics:
  - Data Management
  - Security
  - Security Operations
---

# [Google Security Operations - SIEM Rules](https://www.cloudskillsboost.google/course_templates/690)

**Description:**

Get hands-on experience applying and building rules for Chronicle. You learn what YARA-L is and how to customize & create event rules.

## Using the Chronicle Platform

### Lab - [Chronicle SIEM: Introduction & Single Event Rules](https://www.cloudskillsboost.google/course_templates/690/labs/472959)

In this lab you perform basic configuration tasks within a Chronicle environment instance.

* [ ] [Chronicle SIEM: Introduction & Single Event Rules](../labs/Chronicle-SIEM-Introduction-&-Single-Event-Rules.md)

### Quiz - [Chronicle SIEM: Introduction & Single Event Rules Quiz](https://www.cloudskillsboost.google/course_templates/690/quizzes/472960)

#### Quiz 1.

> [!important]
> **Adding and Modifying rules is accomplished from which screen?**
>
> * [ ] Rules Dashboard
> * [ ] Chronicle Rules
> * [ ] Rules Editor
> * [ ] Enterprise Insights

#### Quiz 2.

> [!important]
> **Which of the following is the correct syntax to use nocase?   **
>
> * [ ] $e.network.ip_protocol = "TCP" nocase
> * [ ] All of the above
> * [ ] target.user.userid = "TIM.SMITH" nocase
> * [ ] metadata.event_type = "USER_LOGIN" nocase

#### Quiz 3.

> [!important]
> **$var is equivalent to**
>
> * [ ] $var > 0
> * [ ] #var <= 1
> * [ ] #var > 0
> * [ ] #var >= 0

#### Quiz 4.

> [!important]
> **Which section stores arbitrary key-value pairs of rule details?**
>
> * [ ] Meta
> * [ ] Event
> * [ ] Option
> * [ ] Outcome

#### Quiz 5.

> [!important]
> **The precedence order for logical operators is**
>
> * [ ] NOT, OR, AND
> * [ ] AND, OR, NOT
> * [ ] OR, AND, NOT
> * [ ] NOT, AND, OR

#### Quiz 6.

> [!important]
> **A new rule has been developed and historical data over the last year needs to be investigated. You must run ______ to perform the investigation.**
>
> * [ ] Retrohunt
> * [ ] Live Status
> * [ ] Test Rule
> * [ ] Alerting

#### Quiz 7.

> [!important]
> **What does the following statement signify?
not all $e.principal.ip = "127.0.0.1"    **
>
> * [ ] checks that no IP addresses match to "127.0.0.1"
> * [ ] checks whether any IP address does not match "127.0.0.1"
> * [ ] checks whether any IP address match "127.0.0.1"
> * [ ] None of the above

#### Quiz 8.

> [!important]
> **Which of the following is the valid syntax when using the any operator?**
>
> * [ ] any $e.target.ip = "127.0.0.1"
> * [ ] None of the above
> * [ ] any $e1.principal.ip = $e2.principal.ip
> * [ ] any $e.principal.ip = $ip

#### Quiz 9.

> [!important]
> **In which section of a YARA-L rule can placeholder variables defined in the events section not be used?**
>
> * [ ] outcome
> * [ ] condition
> * [ ] options
> * [ ] match

#### Quiz 10.

> [!important]
> **Which sections are mandatory for all YARA-L Rules? You can select the multiple values**
>
> * [ ] options
> * [ ] condition
> * [ ] meta
> * [ ] outcome
> * [ ] events
> * [ ] match

### Lab - [Chronicle SIEM: Multi Event Rules](https://www.cloudskillsboost.google/course_templates/690/labs/472961)

In this lab you will learn more about Multi Event Rules of the Chronicle security solution.

* [ ] [Chronicle SIEM: Multi Event Rules](../labs/Chronicle-SIEM-Multi-Event-Rules.md)

### Quiz - [Chronicle SIEM: Multi Event Rules Quiz](https://www.cloudskillsboost.google/course_templates/690/quizzes/472962)

#### Quiz 1.

> [!important]
> **What is the Maximum time range value specified in match section to correlate events**
>
> * [ ] 24 hours
> * [ ] 36 hours
> * [ ] 48 hours
> * [ ] 12 hours

#### Quiz 2.

> [!important]
> **Which of the following is the correct rule which is going to detect whether the user has logged in your enterprise from two or more cities and he is not from the INFORMATION TECHNOLOGY department? **
>
> * [ ] 
  
  rule example {
  
  meta:
     author = "Chronicle"
     severity = "Medium"
  
  events:
     $e1.metadata.event_type = "USER_LOGIN"
     $e1.target.user.userid = $user
     $e1.principal.location.city = $city
  
     $e.graph.entity.user.userid = $user
     $e.graph.metadata.entity_type = "USER"
     ($e.graph.entity.user.department != "INFORMATION TECHNOLOGY")
  
  match:
     $user over 24h
  
  condition:
     $e1 and $e and #city > 1
  }
  

> * [ ] 
  
  rule example {
  
  meta:
     author = "Chronicle"
     severity = "Medium"
  
  events:
     $e1.metadata.event_type = "USER_LOGIN"
     $e1.target.user.userid = $user
     $e1.principal.location.city = $city
  
  match:
     $user over 24h
  
  condition:
     $e1 and #city > 1
  }
  

> * [ ] 
  
  rule example {
  
  meta:
     author = "Chronicle"
     severity = "Medium"
  
  events:
     $e1.metadata.event_type = "USER_LOGIN"
     $e1.target.user.userid = $user
     $e1.principal.location.city = $city
  
     $e.graph.entity.user.userid = $user
     $e.graph.metadata.entity_type = "USER"
     ($e.graph.entity.user.department != " INFO TECH")
  
  match:
     $user over 24h
  
  condition:
     $e1 and $e and #city > 1
  }
  

> * [ ] 
  
  rule example {
  
  meta:
     author = "Chronicle"
     severity = "Medium"
  
  events:
     $e1.metadata.event_type = "USER_LOGIN"
     $e1.target.user.userid = $user
     $e1.principal.location.city = $city
  
     $e.graph.entity.user.userid = $user
     $e.graph.metadata.entity_type = "USER"
     ($e.graph.entity.user.department != "INFORMATION TECHNOLOGY")
  
  match:
     $user over 24h
  
  condition:
     $e1 and #city > 1
  }
  


#### Quiz 3.

> [!important]
> **YARA-L rule can be evaluated using what type of match technique?**
>
> * [ ] None
> * [ ] Hop window
> * [ ] Sliding window
> * [ ] Both

#### Quiz 4.

> [!important]
> **Which of the following is the correct rule to detect multiple events?**
>
> * [ ] 
  
  rule EventRule {
  meta:
      author = "Chronicle"
  
  events:
      $e.metadata.event_type = "USER_LOGIN"
      $e.principal.user.userid = $user
  
  condition:
      #e >= 10
  }
  

> * [ ] 
  
  rule EventRule {
  meta:
     author = "Chronicle"
  
  events:
     $e.metadata.event_type = "USER_LOGIN"
     $e.principal.user.userid = $user
  
  match:
     $user over 10m
  }
  

> * [ ] All of the above
> * [ ] 
  
  rule EventRule {
  meta:
     author = "Chronicle"
  
  events:
     $e.metadata.event_type = "USER_LOGIN"
     $e.principal.user.userid = $user
  
  match:
     $user over 10m
  
  condition:
     #e >= 10
  }
  


#### Quiz 5.

> [!important]
> **If we want to write a rule that must only look for events within a 20 minute window, what section of the rule do you place this condition in?**
>
> * [ ] condition
> * [ ] meta
> * [ ] events
> * [ ] match

#### Quiz 6.

> [!important]
> **Identify the use case of given rule
Rule:  
  rule example {
  meta:
     author = "Chronicle Security"
     severity = "Low"
    
  events:
     $fail.metadata.event_type      = "USER_LOGIN"
     $fail.metadata.vendor_name     = "Microsoft"
     $fail.principal.hostname       = $targetHost
     $fail.target.user.userid       = $targetUser
     $fail.security_result.category = "AUTH_VIOLATION"
     $fail.security_result.action   = "BLOCK"
    
     $fail.metadata.event_timestamp.seconds 
    
     $success.metadata.event_type = "USER_LOGIN"
     $success.target.user.userid = $targetUser
     $success.principal.hostname     = $targetHost
     $success.security_result.action = "ALLOW"
     $success.metadata.product_event_type != "4648"
    
  match:
     $targetUser, $targetHost over 15m
    
  condition:
     #fail > 4 and $success
  }
  
**
>
> * [ ] Detect repeated authentication failure, followed by authentication success.
> * [ ] Detect login success.
> * [ ] None of the above.
> * [ ] Detect authentication success, followed by authentication failure.

#### Quiz 7.

> [!important]
> **
Identify the incorrect event section from the given options. (assuming $e1, $e2, and $e3 are used in the rule)
**
>
> * [ ] 
  
  events:
     $e1.src.ip = $ip
     $e2.target.ip = $ip
     $e3.about.ip = $ip
  

> * [ ] 
  
  events:
     $e1.src.ip = $ip
     $e2.target.ip = $ip
     $e3.about.ip = "192.1.2.0"
  

> * [ ] All of the above
> * [ ] 
  
  events:
     $e1.principal.hostname = $e2.src.hostname
     $e2.principal.ip = $e3.src.ip
  


#### Quiz 8.

> [!important]
> **Identify the use case of given rule
Rule:  
  rule UserCreationThenDeletion {
  meta:
    
  events:
     $create.target.user.userid = $user
     $create.metadata.event_type = "USER_CREATION"
    
     $delete.target.user.userid = $user
     $delete.metadata.event_type = "USER_DELETION"
    
     $create.metadata.event_timestamp.seconds 
        $delete.metadata.event_timestamp.seconds
    
  match:
     $user over 4h
    
  condition:
     $create and $delete
  }
  
**
>
> * [ ] users that have been created and then deleted within 4 hours.
> * [ ] users that have been created within the interval of 4 hours.
> * [ ] None of the above.
> * [ ] users that have been deleted within the interval of 4 hours.

#### Quiz 9.

> [!important]
> **Identify the correct rule definition**
>
> * [ ] 
  
  rule RuleExample {
  meta:
     author = "Chronicle"
  
  events:
     $e1.metadata.product_name = "firewall_1"
     $e1.principal.hostname = $host
  
     $e2.metadata.product_name = "firewall_2"
     $e2.principal.hostname = $host
  
  match:
     $host over 10m after $e1
  
  condition:
     $e1 and !$e2
  }
  

> * [ ] None of the above
> * [ ] 
  
  rule RuleExample {
  meta:
     author = "Chronicle"
  
  events:
     $e1.metadata.product_name = "firewall_1"
     $e1.principal.hostname = $host
  
     $e2.metadata.product_name = "firewall_2"
     $e2.principal.hostname = $host
  
  match:
     $host over 10m
  
  condition:
     $e1 and !$e2
  }
  

> * [ ] Both A & B

#### Quiz 10.

> [!important]
> **Which of the following is correct syntax for a rule which is going to detect whether the user has logged in your enterprise from two or more cities?**
>
> * [ ] None of the above
> * [ ] 
  
  rule DifferentCityLogin {
  meta:
     author = "Chronicle"
     severity = "Low"
  events:
     $udm.metadata.event_type = "USER_LOGIN"
     $udm.principal.user.userid = $user
     $udm.principal.location.city = $city
  
  match:
     $user over 5m
  
  condition:
     $udm and #city > 1
  }
  

> * [ ] 
  
  rule DifferentCityLogin {
  meta:
     author = "Chronicle"
     severity = "Low"
  events:
     $udm.metadata.event_type = "USER_LOGIN"
     $udm.principal.user.userid = $user
     $udm.principal.location.city = $city
  
  match:
     $udm and #city > 1
  
  condition:
     $user over 5m
  }
  

> * [ ] 
  
  rule DifferentCityLogin {
  meta:
  
  events:
     $udm.metadata.event_type = "USER_LOGIN"
     $udm.principal.user.userid = $user
     $udm.principal.location.city = $city
  
  match:
     $user over 5m
     author = "Chronicle"
     severity = "Low"
  
  condition:
     $udm and #city > 1
  }
  


### Lab - [Chronicle SIEM: Outcomes & Functions](https://www.cloudskillsboost.google/course_templates/690/labs/472963)

In this lab you will learn more about Outcomes and Functions of the Chronicle security solution.

* [ ] [Chronicle SIEM: Outcomes & Functions](../labs/Chronicle-SIEM-Outcomes-&-Functions.md)

### Quiz - [Chronicle SIEM: Outcomes & Functions Quiz](https://www.cloudskillsboost.google/course_templates/690/quizzes/472964)

#### Quiz 1.

> [!important]
> **Identify the correct syntax for to work with the list key_servers.**
>
> * [ ] $selection1.principal.hostname in list key_server
> * [ ] $selection1.principal.hostname %key_server
> * [ ] $selection1.principal.hostname in %key_servers
> * [ ] $selection1.principal.hostname in list %key_server

#### Quiz 2.

> [!important]
> **Functions in YARA-L apply to exactly one event**
>

#### Quiz 3.

> [!important]
> **The special field in the outcome section is**
>
> * [ ] $risk_score
> * [ ] $riskScore
> * [ ] $result
> * [ ] $outcome

#### Quiz 4.

> [!important]
> **Identify the correct option which is going to match the event which received the email from altostrat.com(case sensitive) domain.
Option 1: re.regex($e.network.email.from, `\.*altostrat\.com`)
Option 2: $e.network.email.from = /\.*altostrat\.com/**
>
> * [ ] Option 1 & 2 (Both)
> * [ ] Option 2
> * [ ] None of the above options
> * [ ] Option 1

#### Quiz 5.

> [!important]
> **Identify the correct syntax in the events section to use a reference list**
>
> * [ ] All the three options
> * [ ] re.capture($udm.target.process.file.full_path, /.*\\(.*)/) in %processes
> * [ ] $udm.principal.hostname in %machines
> * [ ] $udm.principal.ip in cidr %cidr_reference_list

#### Quiz 6.

> [!important]
> **
  
    function
    use case
  
  
    1) strings.concat(a, b)
    | a) Change text to lowercase
  
  
    2) strings.to_lower(a)
    | b) Change text to uppercase
  
  
    3) strings.to_upper(b)
    | c) Concatenation of  two strings
  **
>
> * [ ] 1->b, 2->c, 3->a
> * [ ] 1->c, 2->b, 3->c
> * [ ] 1->a, 2->b, 3->c
> * [ ] 1->c, 2->a, 3->b

#### Quiz 7.

> [!important]
> **Which of the following is not an aggregate function in the Outcome section?**
>
> * [ ] sum()
> * [ ] count_distinct()
> * [ ] abs()
> * [ ] max()

#### Quiz 8.

> [!important]
> **UDM field $e.principal.hostname returns the value "name". What will the value of $variable become after this function has been processed?
$variable = re.replace($e.principal.hostname, "", "1")?**
>
> * [ ] n1a1m1e1
> * [ ] 1
> * [ ] 1n1a1m1e1
> * [ ] name1

#### Quiz 9.

> [!important]
> **The multi-event rule can be simplified to a single event rule. Which option is syntactically correct when converted to a single event rule?.  
    rule example {
    meta:
       author = "Chronicle"
    
    events:
       $u.udm.principal.hostname = $hostname
    
    match:
       $hostname over 5m
    
    outcome:
       $risk_score = max(if($hostname = "my-hostname", 100, 50))
    
    condition:
       $u
  }
  
**
>
> * [ ] 
  
  rule example {
  meta:
     author = "Chronicle"
  
  events:
     $u.udm.principal.hostname = $hostname
  
  match:
     $hostname over 5m
  
  outcome:
     $risk_score = if($hostname = "my-hostname", 100, 50)
  
  condition:
     $u
  }
  

> * [ ] 
  
  rule example {
  meta:
     author = "Chronicle"
  
  events:
     $u.udm.principal.hostname = $hostname
  
  outcome:
     $risk_score = max(if($hostname = "my-hostname", 100, 50))
  
  condition:
     $u
  }
  

> * [ ]         
  
  rule example {
  meta:
     author = "Chronicle"
  
  events:
     $u.udm.principal.hostname = $hostname
  
  outcome:
     $risk_score = if($hostname = "my-hostname", 100, 50)
  
  condition:
     $u
  }
  

> * [ ] None of the above.

#### Quiz 10.

> [!important]
> **Which of the following is the correct criterion for a rule which is going to detect whether the user has logged in to your enterprise outside working hours? (working hours are from 10:00 to 19:00)**
>
> * [ ] 
  $ts = $e1.metadata.event_timestamp.seconds
  timestamp.get_hour($ts)  18

> * [ ] 
  $ts = $e1.metadata.event_timestamp.seconds
  timestamp.get_hour($ts)  19

> * [ ] 
  $ts = $e1.metadata.event_timestamp
  timestamp.get_hour($ts)  18

> * [ ] 
  $ts = $e1.metadata.event_timestamp.seconds
  timestamp.get_hour($ts) = 10 or timestamp.get_hour($ts) = 19


## Your Next Steps

### Badge - [Course Badge](https://www.cloudskillsboost.google)
