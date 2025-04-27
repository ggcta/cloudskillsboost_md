---
id: 690
name: 'Google Security Operations - SIEM Rules'
datePublished: 2024-05-07
topics:
- Security
- Rules
- SIEM
type: Course
url: https://www.cloudskillsboost.google/course_templates/690
---

# [Google Security Operations - SIEM Rules](https://www.cloudskillsboost.google/course_templates/690)

**Description:**

Get hands-on experience applying and building rules for Chronicle. You learn what YARA-L is and how to customize & create event rules.

## Using the Chronicle Platform

### Lab - [Chronicle SIEM: Introduction & Single Event Rules](https://www.cloudskillsboost.google/course_templates/690/labs/472959)

In this lab you perform basic configuration tasks within a Chronicle environment instance.

- [ ] [Chronicle SIEM: Introduction & Single Event Rules](../labs/Chronicle-SIEM-Introduction-&-Single-Event-Rules.md)

### Quiz - [Chronicle SIEM: Introduction & Single Event Rules Quiz](https://www.cloudskillsboost.google/course_templates/690/quizzes/472960)

#### Quiz 1.

> [!important]
> **Which section stores arbitrary key-value pairs of rule details?**
>
> - [ ] Option
> - [ ] Event
> - [ ] Outcome
> - [ ] Meta

#### Quiz 2.

> [!important]
> **What does the following statement signify?<br />
<code>not all $e.principal.ip = "127.0.0.1"</code>    **
>
> - [ ] checks whether any IP address does not match "127.0.0.1"
> - [ ] checks whether any IP address match "127.0.0.1"
> - [ ] None of the above
> - [ ] checks that no IP addresses match to "127.0.0.1"

#### Quiz 3.

> [!important]
> **A new rule has been developed and historical data over the last year needs to be investigated. You must run ______ to perform the investigation.**
>
> - [ ] Test Rule
> - [ ] Alerting
> - [ ] Retrohunt
> - [ ] Live Status

#### Quiz 4.

> [!important]
> **In which section of a YARA-L rule can placeholder variables defined in the events section not be used?**
>
> - [ ] condition
> - [ ] options
> - [ ] match
> - [ ] outcome

#### Quiz 5.

> [!important]
> **The precedence order for logical operators is**
>
> - [ ] OR, AND, NOT
> - [ ] NOT, AND, OR
> - [ ] NOT, OR, AND
> - [ ] AND, OR, NOT

#### Quiz 6.

> [!important]
> **Which of the following is the valid syntax when using the any operator?**
>
> - [ ] <code>any $e.principal.ip = $ip</code>
> - [ ] None of the above
> - [ ] <code>any $e.target.ip = "127.0.0.1"</code>
> - [ ] <code>any $e1.principal.ip = $e2.principal.ip</code>

#### Quiz 7.

> [!important]
> **Adding and Modifying rules is accomplished from which screen?**
>
> - [ ] Rules Editor
> - [ ] Chronicle Rules
> - [ ] Enterprise Insights
> - [ ] Rules Dashboard

#### Quiz 8.

> [!important]
> **Which of the following is the correct syntax to use nocase?   **
>
> - [ ] <code>metadata.event_type = "USER_LOGIN" nocase</code>
> - [ ] All of the above
> - [ ] <code>$e.network.ip_protocol = "TCP" nocase</code>
> - [ ] <code>target.user.userid = "TIM.SMITH" nocase</code>

#### Quiz 9.

> [!important]
> **Which sections are mandatory for all YARA-L Rules? You can select the multiple values**
>
> - [ ] options
> - [ ] match
> - [ ] outcome
> - [ ] condition
> - [ ] meta
> - [ ] events

#### Quiz 10.

> [!important]
> **$var is equivalent to**
>
> - [ ] #var <= 1
> - [ ] #var > 0
> - [ ] #var >= 0
> - [ ] $var > 0

### Lab - [Chronicle SIEM: Multi Event Rules](https://www.cloudskillsboost.google/course_templates/690/labs/472961)

In this lab you will learn more about Multi Event Rules of the Chronicle security solution.

- [ ] [Chronicle SIEM: Multi Event Rules](../labs/Chronicle-SIEM-Multi-Event-Rules.md)

### Quiz - [Chronicle SIEM: Multi Event Rules Quiz](https://www.cloudskillsboost.google/course_templates/690/quizzes/472962)

#### Quiz 1.

> [!important]
> **If we want to write a rule that must only look for events within a 20 minute window, what section of the rule do you place this condition in?**
>
> - [ ] condition
> - [ ] meta
> - [ ] match
> - [ ] events

#### Quiz 2.

> [!important]
> **Which of the following is correct syntax for a rule which is going to detect whether the user has logged in your enterprise from two or more cities?**
>
> - [ ] <div>
  <code><br />
  rule DifferentCityLogin {<br />
  meta:<br />
    &ensp;author = "Chronicle"<br />
    &ensp;severity = "Low"<br />
  events:<br />
    &ensp;$udm.metadata.event_type = "USER_LOGIN"<br />
    &ensp;$udm.principal.user.userid = $user<br />
    &ensp;$udm.principal.location.city = $city<br />
  <br/>
  match:<br />
    &ensp;$user over 5m<br />
  <br/>
  condition:<br />
    &ensp;$udm and #city > 1<br />
  }
  </code>
</div>
> - [ ] <div>
  <code><br />
  rule DifferentCityLogin {<br />
  meta:<br />
  <br/>
  events:<br />
    &ensp;$udm.metadata.event_type = "USER_LOGIN"<br />
    &ensp;$udm.principal.user.userid = $user<br />
    &ensp;$udm.principal.location.city = $city<br />
  <br/>
  match:<br />
    &ensp;$user over 5m<br />
    &ensp;author = "Chronicle"<br />
    &ensp;severity = "Low"<br />
  <br/>
  condition:<br />
    &ensp;$udm and #city > 1<br />
  }
  </code>
</div>
> - [ ] <div>
  <code><br />
  rule DifferentCityLogin {<br />
  meta:<br />
    &ensp;author = "Chronicle"<br />
    &ensp;severity = "Low"<br />
  events:<br />
    &ensp;$udm.metadata.event_type = "USER_LOGIN"<br />
    &ensp;$udm.principal.user.userid = $user<br />
    &ensp;$udm.principal.location.city = $city<br />
  <br/>
  match:<br />
    &ensp;$udm and #city > 1<br />
  <br/>
  condition:<br />
    &ensp;$user over 5m<br />
  }
  </code>
</div>
> - [ ] None of the above

#### Quiz 3.

> [!important]
> **Identify the correct rule definition**
>
> - [ ] None of the above
> - [ ] Both A & B
> - [ ] <div>
  <code><br />
  rule RuleExample {<br />
  meta:<br />
    &ensp;author = "Chronicle"<br />
  <br/>
  events:<br />
    &ensp;$e1.metadata.product_name = "firewall_1"<br />
    &ensp;$e1.principal.hostname = $host<br />
  <br/>
    &ensp;$e2.metadata.product_name = "firewall_2"<br />
    &ensp;$e2.principal.hostname = $host<br />
  <br/>
  match:<br />
    &ensp;$host over 10m after $e1<br />
  <br/>
  condition:<br />
    &ensp;$e1 and !$e2<br />
  }
  </code>
</div>
> - [ ] <div>
  <code><br />
  rule RuleExample {<br />
  meta:<br />
    &ensp;author = "Chronicle"<br />
  <br/>
  events:<br />
    &ensp;$e1.metadata.product_name = "firewall_1"<br />
    &ensp;$e1.principal.hostname = $host<br />
  <br/>
    &ensp;$e2.metadata.product_name = "firewall_2"<br />
    &ensp;$e2.principal.hostname = $host<br />
  <br/>
  match:<br />
    &ensp;$host over 10m<br />
  <br/>
  condition:<br />
    &ensp;$e1 and !$e2<br />
  }
  </code>
</div>

#### Quiz 4.

> [!important]
> **Which of the following is the correct rule which is going to detect whether the user has logged in your enterprise from two or more cities and he is not from the INFORMATION TECHNOLOGY department? **
>
> - [ ] <div>
  <code><br />
  rule example {<br />
  <br/>
  meta:<br />
    &ensp;author = "Chronicle"<br />
    &ensp;severity = "Medium"<br />
  <br/>
  events:<br />
    &ensp;$e1.metadata.event_type = "USER_LOGIN"<br />
    &ensp;$e1.target.user.userid = $user<br />
    &ensp;$e1.principal.location.city = $city<br />
  <br/>
    &ensp;$e.graph.entity.user.userid = $user<br />
    &ensp;$e.graph.metadata.entity_type = "USER"<br />
    &ensp;($e.graph.entity.user.department != "INFORMATION TECHNOLOGY")<br />
  <br/>
  match:<br />
    &ensp;$user over 24h<br />
  <br/>
  condition:<br />
    &ensp;$e1 and $e and #city > 1<br />
  }
  </code>
</div>
> - [ ] <div>
  <code><br />
  rule example {<br />
  <br/>
  meta:<br />
    &ensp;author = "Chronicle"<br />
    &ensp;severity = "Medium"<br />
  <br/>
  events:<br />
    &ensp;$e1.metadata.event_type = "USER_LOGIN"<br />
    &ensp;$e1.target.user.userid = $user<br />
    &ensp;$e1.principal.location.city = $city<br />
  <br/>
    &ensp;$e.graph.entity.user.userid = $user<br />
    &ensp;$e.graph.metadata.entity_type = "USER"<br />
    &ensp;($e.graph.entity.user.department != "INFORMATION TECHNOLOGY")<br />
  <br/>
  match:<br />
    &ensp;$user over 24h<br />
  <br/>
  condition:<br />
    &ensp;$e1 and #city > 1<br />
  }
  </code>
</div>
> - [ ] <div>
  <code><br />
  rule example {<br />
  <br/>
  meta:<br />
    &ensp;author = "Chronicle"<br />
    &ensp;severity = "Medium"<br />
  <br/>
  events:<br />
    &ensp;$e1.metadata.event_type = "USER_LOGIN"<br />
    &ensp;$e1.target.user.userid = $user<br />
    &ensp;$e1.principal.location.city = $city<br />
  <br/>
  match:<br />
    &ensp;$user over 24h<br />
  <br/>
  condition:<br />
    &ensp;$e1 and #city > 1<br />
  }
  </code>
</div>
> - [ ] <div>
  <code><br />
  rule example {<br />
  <br/>
  meta:<br />
    &ensp;author = "Chronicle"<br />
    &ensp;severity = "Medium"<br />
  <br/>
  events:<br />
    &ensp;$e1.metadata.event_type = "USER_LOGIN"<br />
    &ensp;$e1.target.user.userid = $user<br />
    &ensp;$e1.principal.location.city = $city<br />
  <br/>
    &ensp;$e.graph.entity.user.userid = $user<br />
    &ensp;$e.graph.metadata.entity_type = "USER"<br />
    &ensp;($e.graph.entity.user.department != " INFO TECH")<br />
  <br/>
  match:<br />
    &ensp;$user over 24h<br />
  <br/>
  condition:<br />
    &ensp;$e1 and $e and #city > 1<br />
  }
  </code>
</div>

#### Quiz 5.

> [!important]
> **Which of the following is the correct rule to detect multiple events?**
>
> - [ ] <div>
  <code><br />
  rule EventRule {<br />
  meta:<br />
     &ensp;author = "Chronicle"<br />
  <br/>
  events:<br />
     &ensp;$e.metadata.event_type = "USER_LOGIN"<br />
     &ensp;$e.principal.user.userid = $user<br />
  <br/>
  condition:<br />
     &ensp;#e >= 10<br />
  }
  </code>
</div>
> - [ ] <div>
  <code><br />
  rule EventRule {<br />
  meta:<br />
    &ensp;author = "Chronicle"<br />
  <br/>
  events:<br />
    &ensp;$e.metadata.event_type = "USER_LOGIN"<br />
    &ensp;$e.principal.user.userid = $user<br />
  <br/>
  match:<br />
    &ensp;$user over 10m<br />
  <br/>
  condition:<br />
    &ensp;#e >= 10<br />
  }
  </code>
</div>
> - [ ] <div>
  <code><br />
  rule EventRule {<br />
  meta:<br />
    &ensp;author = "Chronicle"<br />
  <br/>
  events:<br />
    &ensp;$e.metadata.event_type = "USER_LOGIN"<br />
    &ensp;$e.principal.user.userid = $user<br />
  <br/>
  match:<br />
    &ensp;$user over 10m<br />
  }
  </code>
</div>
> - [ ] All of the above

#### Quiz 6.

> [!important]
> **
Identify the incorrect event section from the given options. (assuming $e1, $e2, and $e3 are used in the rule)
**
>
> - [ ] <div>
  <code><br />
  events:<br />
    &ensp;$e1.src.ip = $ip<br />
    &ensp;$e2.target.ip = $ip<br />
    &ensp;$e3.about.ip = "192.1.2.0"
  </code>
</div>
> - [ ] <div>
  <code><br />
  events:<br />
    &ensp;$e1.principal.hostname = $e2.src.hostname<br />
    &ensp;$e2.principal.ip = $e3.src.ip
  </code>
</div>
> - [ ] All of the above
> - [ ] <div>
  <code><br />
  events:<br />
    &ensp;$e1.src.ip = $ip<br />
    &ensp;$e2.target.ip = $ip<br />
    &ensp;$e3.about.ip = $ip
  </code>
</div>

#### Quiz 7.

> [!important]
> **YARA-L rule can be evaluated using what type of match technique?**
>
> - [ ] None
> - [ ] Both
> - [ ] Hop window
> - [ ] Sliding window

#### Quiz 8.

> [!important]
> **What is the Maximum time range value specified in match section to correlate events**
>
> - [ ] 36 hours
> - [ ] 12 hours
> - [ ] 24 hours
> - [ ] 48 hours

#### Quiz 9.

> [!important]
> **Identify the use case of given rule<br />
Rule:
<div>
  <code><br />
  rule UserCreationThenDeletion {<br />
  meta:<br />
    <br/>
  events:<br />
    &ensp;$create.target.user.userid = $user<br />
    &ensp;$create.metadata.event_type = "USER_CREATION"<br />
    <br/>
    &ensp;$delete.target.user.userid = $user<br />
    &ensp;$delete.metadata.event_type = "USER_DELETION"<br />
    <br/>
    &ensp;$create.metadata.event_timestamp.seconds <=<br />
      &ensp;&ensp;$delete.metadata.event_timestamp.seconds<br />
    <br/>
  match:<br />
    &ensp;$user over 4h<br />
    <br/>
  condition:<br />
    &ensp;$create and $delete<br />
  }
  </code>
</div>**
>
> - [ ] users that have been created and then deleted within 4 hours.
> - [ ] users that have been deleted within the interval of 4 hours.
> - [ ] users that have been created within the interval of 4 hours.
> - [ ] None of the above.

#### Quiz 10.

> [!important]
> **Identify the use case of given rule<br />
Rule:
<div>
  <code><br />
  rule example {<br />
  meta:<br />
    &ensp;author = "Chronicle Security"<br />
    &ensp;severity = "Low"<br />
    <br/>
  events:<br />
    &ensp;$fail.metadata.event_type      = "USER_LOGIN"<br />
    &ensp;$fail.metadata.vendor_name     = "Microsoft"<br />
    &ensp;$fail.principal.hostname       = $targetHost<br />
    &ensp;$fail.target.user.userid       = $targetUser<br />
    &ensp;$fail.security_result.category = "AUTH_VIOLATION"<br />
    &ensp;$fail.security_result.action   = "BLOCK"<br />
    <br/>
    &ensp;$fail.metadata.event_timestamp.seconds <= $success.metadata.event_timestamp.seconds<br />
    <br/>
    &ensp;$success.metadata.event_type = "USER_LOGIN"<br />
    &ensp;$success.target.user.userid = $targetUser<br />
    &ensp;$success.principal.hostname     = $targetHost<br />
    &ensp;$success.security_result.action = "ALLOW"<br />
    &ensp;$success.metadata.product_event_type != "4648"<br />
    <br/>
  match:<br />
    &ensp;$targetUser, $targetHost over 15m<br />
    <br/>
  condition:<br />
    &ensp;#fail > 4 and $success<br />
  }
  </code>
</div>**
>
> - [ ] Detect login success.
> - [ ] Detect authentication success, followed by authentication failure.
> - [ ] None of the above.
> - [ ] Detect repeated authentication failure, followed by authentication success.

### Lab - [Chronicle SIEM: Outcomes & Functions](https://www.cloudskillsboost.google/course_templates/690/labs/472963)

In this lab you will learn more about Outcomes and Functions of the Chronicle security solution.

- [ ] [Chronicle SIEM: Outcomes & Functions](../labs/Chronicle-SIEM-Outcomes-&-Functions.md)

### Quiz - [Chronicle SIEM: Outcomes & Functions Quiz](https://www.cloudskillsboost.google/course_templates/690/quizzes/472964)

#### Quiz 1.

#### Quiz 1.

> [!important]
> **The multi-event rule can be simplified to a single event rule. Which option is syntactically correct when converted to a single event rule?.<br />
<div>
  <code><br />
    rule example {<br />
    meta:<br />
      &ensp;author = "Chronicle"<br />
    <br/>
    events:<br />
      &ensp;$u.udm.principal.hostname = $hostname<br />
    <br/>
    match:<br />
      &ensp;$hostname over 5m<br />
    <br/>
    outcome:<br />
      &ensp;$risk_score = max(if($hostname = "my-hostname", 100, 50))<br />
    <br/>
    condition:<br />
      &ensp;$u<br />
  }
  </code>
</div>**
>
> - [ ] None of the above.
> - [ ] <div>        
  <code><br />
  rule example {<br />
  meta:<br />
    &ensp;author = "Chronicle"<br />
  <br/>
  events:<br />
    &ensp;$u.udm.principal.hostname = $hostname<br />
  <br/>
  outcome:<br />
    &ensp;$risk_score = if($hostname = "my-hostname", 100, 50)<br />
  <br/>
  condition:<br />
    &ensp;$u<br />
  }
  </code>
</div>
> - [ ] <div>
  <code><br />
  rule example {<br />
  meta:<br />
    &ensp;author = "Chronicle"<br />
  <br/>
  events:<br />
    &ensp;$u.udm.principal.hostname = $hostname<br />
  <br/>
  match:<br />
    &ensp;$hostname over 5m<br />
  <br/>
  outcome:<br />
    &ensp;$risk_score = if($hostname = "my-hostname", 100, 50)<br />
  <br/>
  condition:<br />
    &ensp;$u<br />
  }
  </code>
</div>
> - [ ] <div>
  <code><br />
  rule example {<br />
  meta:<br />
    &ensp;author = "Chronicle"<br />
  <br/>
  events:<br />
    &ensp;$u.udm.principal.hostname = $hostname<br />
  <br/>
  outcome:<br />
    &ensp;$risk_score = max(if($hostname = "my-hostname", 100, 50))<br />
  <br/>
  condition:<br />
    &ensp;$u<br />
  }
  </code>
</div>

#### Quiz 2.

> [!important]
> **Which of the following is the correct criterion for a rule which is going to detect whether the user has logged in to your enterprise outside working hours? (working hours are from 10:00 to 19:00)**
>
> - [ ] <div>
  <code>$ts = $e1.metadata.event_timestamp</code><br />
  <code>timestamp.get_hour($ts) < 10 or timestamp.get_hour($ts) > 18</code>
</div>
> - [ ] <div>
  <code>$ts = $e1.metadata.event_timestamp.seconds</code><br />
  <code>timestamp.get_hour($ts) < 11 or timestamp.get_hour($ts) > 19</code>
</div>
> - [ ] <div>
  <code>$ts = $e1.metadata.event_timestamp.seconds</code><br />
  <code>timestamp.get_hour($ts) < 10 or timestamp.get_hour($ts) > 18</code>
</div>
> - [ ] <div>
  <code>$ts = $e1.metadata.event_timestamp.seconds</code><br />
  <code>timestamp.get_hour($ts) = 10 or timestamp.get_hour($ts) = 19</code>
</div>

#### Quiz 3.

> [!important]
> **<table>
  <tr>
    <td><b>function</b></td>
    <td><b>use case</b></td>
  </tr>
  <tr>
    <td>1) strings.concat(a, b)</td>
    <td>| a) Change text to lowercase</td>
  </tr>
  <tr>
    <td>2) strings.to_lower(a)</td>
    <td>| b) Change text to uppercase</td>
  </tr>
  <tr>
    <td>3) strings.to_upper(b)</td>
    <td>| c) Concatenation of  two strings</td>
  </tr>**
>
> - [ ] 1->a, 2->b, 3->c
> - [ ] 1->b, 2->c, 3->a
> - [ ] 1->c, 2->a, 3->b
> - [ ] 1->c, 2->b, 3->c

#### Quiz 4.

> [!important]
> **UDM field $e.principal.hostname returns the value "name". What will the value of $variable become after this function has been processed?
<code>$variable = re.replace($e.principal.hostname, "", "1")</code>?**
>
> - [ ] 1n1a1m1e1
> - [ ] 1
> - [ ] n1a1m1e1
> - [ ] name1

#### Quiz 5.

> [!important]
> **The special field in the outcome section is**
>
> - [ ] $result
> - [ ] $outcome
> - [ ] $riskScore
> - [ ] $risk_score

#### Quiz 6.

> [!important]
> **Which of the following is not an aggregate function in the Outcome section?**
>
> - [ ] abs()
> - [ ] sum()
> - [ ] max()
> - [ ] count_distinct()

#### Quiz 7.

> [!important]
> **Identify the correct syntax in the events section to use a reference list**
>
> - [ ] <code>$udm.principal.ip in cidr %cidr_reference_list</code>
> - [ ] <code>$udm.principal.hostname in %machines</code>
> - [ ] All the three options
> - [ ] <code>re.capture($udm.target.process.file.full_path, /.*\\(.*)/) in %processes</code>

#### Quiz 8.

> [!important]
> **Identify the correct syntax for to work with the list key_servers.**
>
> - [ ] $selection1.principal.hostname in %key_servers
> - [ ] $selection1.principal.hostname in list %key_server
> - [ ] $selection1.principal.hostname in list key_server
> - [ ] $selection1.principal.hostname %key_server

#### Quiz 9.

> [!important]
> **Identify the correct option which is going to match the event which received the email from altostrat.com(case sensitive) domain.
Option 1: <code>re.regex($e.network.email.from, `\.*altostrat\.com`)</code>
Option 2: <code>$e.network.email.from = /\.*altostrat\.com/</code>**
>
> - [ ] Option 1
> - [ ] Option 2
> - [ ] None of the above options
> - [ ] Option 1 & 2 (Both)

## Your Next Steps

### Badge - [Course Badge](https://www.cloudskillsboost.googleNone)
