# Recipe App API

Recipe App API created with Django Rest Framework, PostgreSQL, Docker, Travis CI &amp; TDD

### Docker Commands

- `docker build .`: Build dockerfile in current directory.
- `docker-compose build`: Build docker-compose.
- `docker-compose run app sh -c "django-admin.py startproject app ."`: Create new project on app folder in current directory.

### Libraries/Dependencies

- [Flake8](https://pypi.org/project/flake8/): Best Python linter.
  - PEP8: Python Code Stardard
    - [Spanish Explain](https://bioinf.comav.upv.es/courses/linux/python/estilo.html#:~:text=La%20comunidad%20de%20usuarios%20de,completo%20se%20denomina%20PEP%208.)
    - [Official Doc](https://www.python.org/dev/peps/pep-0008/)

### Testing

- How does Django determine where to look for tests?:
  Django searches for any Python module starting with "test". This is why you can store your tests in "tests.py" or "tests/test_something.py"
