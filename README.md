django-mixout
=============

MixoutMixin is a Django mixin that cancels out any functionality that it could
potentially add.

Usage
-----
To use the `MixoutMixin`, just use it like any other mixin in your Django
views.  For example, you can do this:

```python
class AboutView(MixoutMixin, TemplateView):
    template_name = "about.html"
```

This is equivalent to:

```python
class AboutView(TemplateView):
    template_name = "about.html"
```

Credits
-------

I'd like to thank [Ulfur Kristjansson](http://github.com/ulfur) for the
original idea and for helping me out with the design and architecture.
