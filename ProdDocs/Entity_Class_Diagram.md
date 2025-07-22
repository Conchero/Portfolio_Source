``` mermaid

---
title : Portfolio entity class Diagram
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
    - Carousel carousel
}

class Carousel{
    - int id
    - string [] picturesArray
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
Project "*" --> "1" Carousel
Stack "*" --> "1" Category

