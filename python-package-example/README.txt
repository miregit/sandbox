run:
/Users/michaelh/work/data/sandbox/python-package-example
python
import myPackage
print myPackage.somePython.fahrToKelv(32)

upload:
setup.py => change version number
python setup.py sdist
ls -la dist
python setup.py sdist upload -r local

install:
pip install hello-from-secret-unicorns

list:
pip list

uninstall:
pip uninstall hello-from-secret-unicorns

search:
pip search "solima-hello" --verbose -i https://huttermann.jfrog.io/huttermann/api/pypi/pypi/ | grep -i solima-hello
pip install solima-hello
pip list | grep solima

config:
/Users/michaelh/.pip/pip.conf

resources:
https://www.jfrog.com/confluence/display/RTF/PyPI+Repositories 

