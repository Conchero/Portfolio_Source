```mermaid

---
title: Controller Class Diagram
---

classDiagram

class LaravelRessource{
    create()
    edit()
    delete()
    view()
}

class ProjectController {
    index()
}

class TechnologyController

class CategoryController



ProjectController --() LaravelRessource
TechnologyController --() LaravelRessource - Exept_View