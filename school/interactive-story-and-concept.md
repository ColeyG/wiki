# Interactive Story & Concept

## Week 2

- Planning capstone/thesis
  - Create 2/3 ideas to be discussed with profs

## Week 5

- Thesis
  - Decide stack
  - Generate three ideas
  - Concept planned and presented in term 1

Ideas:

- Card game via react
  - Riposte
  - Deployed via electron
- Python Living Art Gallery
  - [example](http://themes.fxoffice.net/lorem/photographer/index.html)
  - ML Integration
  - Fractals
  - Fish Tank
- HTML 5 Store
  - A gallery of HTML layouts for purchase
  - Users can post & sell HTML 5 Layouts

Thesis Planning Doc:

- Elevator Pitch
  - Who/what is the app for?
- Competitive Analysis
  - Why do we need it
- Core Functionality
  - Scope setting
- Map & Wireframe
- Tech
- UI Concepts
- Timesheets & Workback

## Week 8

- Thesis Research Project
  - Functionality Map
    - Presented in a wireframe and flowchart
    - Each step and its code considerations
      - IE: login/register posts data
  - Executive Summary
  - Use Case Scenario
  - Competitive Analysis

- MongoDB beginning
  - Mongo is structure-less
    - Mongo doesn't have types, IE int, char, etc

## Week 9

- `sudo apt install mongodb-clients`
- `sudo apt install mongodb-server-core`

- Commands:
  - `show dbs`
  - `use [db]`
  - `show collections`
  - Create new collections with entry: `db.students.insert({lname:"Jones",fname:"Indiana",image:"wjones.jpg"})`
  - Select *: `db.students.find().pretty()`
  - select * from [] where lname like '%ones': `db.students.find({lname:/ones/}).pretty()`
