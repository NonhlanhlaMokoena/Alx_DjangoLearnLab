# CRUD Operations Documentation

## Create

```python
from bookshelf.models import Book
book = Book.objects.create(title="1984", author="George Orwell", publication_year=1949)
book
```

### Expected Output
<Book: 1984>

---

## Retrieve

```python
Book.objects.all()
```

### Expected Output
<QuerySet [<Book: 1984>]>

---

## Update

```python
book.title = "Nineteen Eighty-Four"
book.save()
book
```

### Expected Output
<Book: Nineteen Eighty-Four>

---

## Delete

```python
book.delete()
Book.objects.all()
```

### Expected Output
<QuerySet []>
