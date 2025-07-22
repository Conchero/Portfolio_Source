``` mermaid

---
title : Portfolio entity class Diagram
---

classDiagram

note "int xID (mysql architecture) || <T> attribute (laravel architecture)"

class Project {
    - int id
    - string title 
    - string slug
    - string type
    - string mainPictureURL
    - DateTime startTime
    - Date endTime
    - string team
    - text projectDescription
    - text developmentDescription
    - ProjectStack[] stackArray
    - ProjectCarousel carousel

    + getter_setter()
}

namespace Database Relevent{

class ProjectStack{
    int id
    string slug 
    int projectID || Project project
    int technologyID  || TechnologytechnologyArray 

    + getter_setter()
}

class ProjectCarousel{
    int id
    string slug 
    int projectID || Project project
    int carouselID || Carousel carousel 

    + getter_setter()
}
}

class Carousel{
    - int id
    - string slug
    - int currentIndex
    - float deltaTime
    - float timeBefore
    - string[] items

    + getter_setter()
    + AddPicture()
    + RemovePictureAt(int _id)
    + GoToNextCarouselItem()
}



class Technology{
    - int id
    - string slug
    - string Name
    - int categoryID || Category category
}


class Category{
    - int id
    - string slug
    - string Name
}


Project "*" --> "1" ProjectStack
ProjectStack "*" --> "*" Technology
Project "*" --> "1" ProjectCarousel
ProjectCarousel "*" --> "*" Carousel
Technology "*" --> "1" Category

