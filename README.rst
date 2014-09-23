===========
pyodcompare
===========

Provides a command line and a class
to generate an odt file wich is a comparison between two documents.

You need a soffice / libreoffice service listening on a port (2002 by default)

	>>> from pyodcompare import DocumentCompare
	>>> compare = DocumentCompare(listener=('localhost', 2002))
	>>> compare.compare('reportV2.doc', 'reportV1.doc', 'reportdiff.odt')

This creates the file reportdiff.odt with a comparaison of reportV2.doc (new )
reportV1.doc (original version)

This uses UNO bridge

Credits
-------

Thomas Desvenain thomas.desvenain@gmail.com

This product is based on the model of PyODConverter
_`https://pypi.python.org/pypi/PyODConverter`

The code has been inspired by this script :
_`http://win32com.goermezer.de/content/view/193/274/`
