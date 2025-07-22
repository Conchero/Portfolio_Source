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

class FilterController

class CategoryController

ProjectController --() LaravelRessource
FilterController --() LaravelRessource - Exept View