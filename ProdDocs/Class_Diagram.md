``` mermaid

---
title : Portfolio class Diagram
---

classDiagram

class Project {
    - int id
    - string title 
    - string type
    - Stack[] stackArray
    - string mainPictureURL
    - DateTime startTime
    - Date endTime
    - string team
    - text projectDescription
    - text developmentDescription
    - string[] picturesArray
}


class Stack{
    - int id
    - string Name
    - Category category
}


class Category{
    - int id
    - string Name
}


Project "*" --> "*" Stack
Stack "*" --> "1" Category