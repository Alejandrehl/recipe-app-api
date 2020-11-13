# Recipe App API

Recipe App API created with Django Rest Framework, PostgreSQL, Docker, Travis CI &amp; TDD

### Docker Commands

- `docker build .`: Build dockerfile in current directory.
- `docker-compose build`: Build docker-compose.
- `docker-compose run app sh -c "django-admin.py startproject app ."`: Create new project called app inside app folder.
- `docker-compose run app sh -c "python manage.py startapp core"`: Create new project called core on inside app folder.
- `docker-compose run app sh -c "python manage.py test"`: Run tests.
- `docker-compose run app sh -c "python manage.py makemigrations MIGRATIONNAME"`: Create a new migration
- `docker-compose up`: Run project with docker-compose file definition.
- `docker-compose run app sh -c "python manage.py test && flake8"`: Run tests with linter flake8.
- `docker-compose run app sh -c "python manage.py createsuperuser"`: Create super user.

### Libraries/Dependencies

- [Flake8](https://pypi.org/project/flake8/): Best Python linter.
  - PEP8: Python Code Stardard
    - [Spanish Explain](https://bioinf.comav.upv.es/courses/linux/python/estilo.html#:~:text=La%20comunidad%20de%20usuarios%20de,completo%20se%20denomina%20PEP%208.)
    - [Official Doc](https://www.python.org/dev/peps/pep-0008/)

### Testing

- How does Django determine where to look for tests?:
  Django searches for any Python module starting with "test". This is why you can store your tests in "tests.py" or "tests/test_something.py"

- Why would you use mocking?
  Mocking is used to isolate the specific code to be tested and to avoid unintended consequences of running your unit tests.

- When writing unit tests, you should never:
  Depend on external services.

# [¿Qué es un Diccionario de datos en Python?](https://devcode.la/tutoriales/diccionarios-en-python/#:~:text=Un%20Diccionario%20es%20una%20estructura,listas%20e%20incluso%20otras%20funciones.&text=Para%20definir%20un%20diccionario%2C%20se,listado%20de%20valores%20entre%20llaves.)

```python
diccionario = {'nombre' : 'Carlos', 'edad' : 22, 'cursos': ['Python','Django','JavaScript'] }

print diccionario['nombre'] #Carlos
print diccionario['edad']#22
print diccionario['cursos'] #['Python','Django','JavaScript']

print diccionario['cursos'][0]#Python
print diccionario['cursos'][1]#Django
print diccionario['cursos'][2]#JavaScript

for key in diccionario:
  print key, ":", diccionario[key]
```
