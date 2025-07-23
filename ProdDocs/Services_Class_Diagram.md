```mermaid

---
title: Services Class Diagram
---

classDiagram

class FileUploadServices{
    - Upload(File _file)
    - Compress(File _file)
    - Delete(string _name)
}


class MailServices{
     SendMail(string _subject, string message)
}


