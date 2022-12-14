# Software Architecture case_studies
Software architecture case studies lesson -Memi Lavi
#  Section 3: Case Study #1 (Dunderly)
## 3.1 Introduction
Dunderly operaions
1. Sells paper supplies (printed paper, envelopes)
2. Needs a new HR System
3. Managing employees (salaries, vacations, payments)

## 3.2 Understanding the requirements
the first step in architecting a software is to understand the requirements
> There 2 types of requirements -
 1. Functional requirements: These are what the system should do
2. Non functional requirments: These are what the system should deal with.

##  Functional requirement of the dunderly system
 Mostly the functional requirements are specified by the users
 - Web based
 - Perform CRUD operations on employees
   - 1. Allow manager to ask for employees salary change
   - 2. Allow HR manager to approve or reject request
 - Manage vacation days
 - Use external system for payment
## Non function requirements 
The first thing to understand about the functional requirement is what we already know about the non functional requirements
> What we already know
  > Classic information sysstem. It's just simple and nothing complicated involving too much moving data
  > Not a lot of users
  > NOt a lot of data
  > Interface to external system. (We have to be careful of interfacing with legacy systems; they can be too problematic)
> Next as what we need to know from the custom
  > 1. How many concurrent users. (this helps us to know the load requirement of the system)
  > 2. How many employees. (large number means large data volumes)
  > 3. What do we know about the external payment system. (What data, how to parse data, how to communicate with the external system)

## 3.1 Logging

