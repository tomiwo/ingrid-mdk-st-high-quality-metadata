
====================
Blick in die Zukunft
====================

Geodaten
--------

**Datenbereitstellung über Geodatendienste oder Schnittstellen (API)**

In Zukunft werden die bestehenden Standards durch neue ergänzt oder ersetzt. Im Folgenden werden die wichtigsten dieser neuen Standards beschrieben, die sich derzeit in der Entwicklung befinden.

----------------------------------------------------------------------------------------------

OGC APIs
""""""""

Die OGC APIs sind eine Familie von Standards, die vom `Open Geospatial Consortium (OGC) <https://ogcapi.ogc.org/#standards>`_ entwickelt wurden, um den Zugang und die Nutzung von Geodaten über das Web zu vereinfachen und zu standardisieren. Diese APIs sind modular aufgebaut und definieren wiederverwendbare Bausteine für raumbezogene Web-APIs.


Hauptmerkmale
^^^^^^^^^^^^^

- **Standardisierung:** OGC APIs folgen einer einheitlichen Struktur, die auf Web-Standards wie HTTP und OpenAPI basiert.
- **Modularität:** Die Standards sind in verschiedene Teile gegliedert, die jeweils spezifische Funktionen abdecken.
- **Interoperabilität:** Sie ermöglichen eine konsistente Interaktion mit Geodaten über verschiedene Systeme hinweg.


Kernfunktionen
^^^^^^^^^^^^^^

- **Datenzugriff:** OGC APIs ermöglichen das Abrufen, Erstellen und Ändern von Geodaten.
- **Abfragemöglichkeiten:** Sie bieten Funktionen zum Filtern und Abfragen von Daten.
- **Formatunterstützung:** Antworten werden typischerweise in JSON oder HTML geliefert.

.. note:: OGC APIs sind eine Weiterentwicklung älterer Standards und sollen die Integration von Geodaten in moderne Anwendungen erleichtern.


---------------------------------------------------------------------------------------------


Welche APIs ersetzen welche Standards?
""""""""""""""""""""""""""""""""""""""


OGC API - Records
^^^^^^^^^^^^^^^^^

Die OGC API - Records soll den Catalogue Service for the Web (CSW) ersetzen und dient der Suche und Abfrage von Metadaten.


OGC API - Features
^^^^^^^^^^^^^^^^^^

Die OGC API - Features ersetzt den Web Feature Service (WFS). Sie ermöglicht das Erstellen, Ändern und Abfragen von räumlichen Daten im Web.

.. note:: Einige Länder haben bereits OGC-API - Features veröffentlicht (z.B. RP, NRW, SL, HH), wobei sich die APIs in ihrer Struktur unterscheiden. Einige APIs bieten einen direkten Datendownload an (z.B. RP, SL), andere sind kaskadierend aufgebaut (HH), hier gelangt man beim Aufruf der API auf eine Landingpage, auf der die Daten zum Download angeboten werden. Aus diesem Grund werden in der Suche weniger Treffer angezeigt.


OGC API - Maps
^^^^^^^^^^^^^^

Die OGC API - Maps soll den Web Map Service (WMS) ersetzen. Sie ermöglicht die Darstellung von digitalen Karten in Kartenviewern.


OGC API - Tiles
^^^^^^^^^^^^^^^^

Die OGC API - Tiles ist der Nachfolger des Web Map Tile Service (WMTS). Sie unterstützt verschiedene Formen gekachelter Geodaten, einschließlich Vektorkacheln, Karten und Bilder.

----------------------------------------------------------------------------------------------


Alternative Encoding
""""""""""""""""""""

GeoJSON und GeoPackage werden oft als alternative Encodings zu traditionellen GIS-Formaten wie GML oder Shapefile genutzt, insbesondere bei INSPIRE-Daten oder in Open-Data-Initiativen. Der Begriff „alternatives Encoding” bedeutet, dass anstelle des offiziellen Standardformats (bei INSPIRE typischerweise GML) ein anderes Format verwendet wird, das sich in der Praxis besser nutzen lässt, zum Beispiel GeoJSON für Webanwendungen oder GeoPackage für Desktop- und mobile GIS-Software. Alternative Encodings erhöhen die Datenzugänglichkeit, Verarbeitungsleistung und Interoperabilität, beispielsweise durch kompaktere und leichter handhabbare Dateien oder eine bessere Unterstützung in modernen Tools. Durch alternative Encodings können dieselben Geodaten flexibler verteilt werden, ohne dass die semantische Information verändert wird. Es wird lediglich das Format angepasst, um spezielle Anwendungsanforderungen oder technische Umgebungen besser zu bedienen.


GeoJSON
^^^^^^^

**GeoJSON** ist ein textbasiertes, leichtgewichtiges Austauschformat, das besonders für Webanwendungen und APIs geeignet ist und mit zahlreichen Plattformen interoperabel ist.


GeoPackage
^^^^^^^^^^

**GeoPackage** ist ein Datei-basiertes Datenbankformat auf SQLite-Basis, das Vektordaten, Rasterdaten, Sachdaten und Metadaten effizient und leistungsfähig in nur einer Datei speichert. Dies ist besonders vorteilhaft für größere oder komplexere Geodatensätze.


.. note:: GeoSN (Sachsen) setzt beispielsweise auf alternatives Encoding.


Online-Veranstaltung der GDI-DE: `2025-11-13 - GDI-DE4EU <https://wiki.gdi-de.org/spaces/insp/pages/1454243908/2025-11-13+GDI-DE4EU>`_

----------------------------------------------------------------------------------------------


STAC-Standard
"""""""""""""

STAC (SpatioTemporal Asset Catalog) ist ein Standard für Geodaten, der es ermöglicht, raumzeitliche Daten (Raster- und Vektordaten) einheitlich, standardisiert und einfach auffindbar zu machen. Es definiert ein interoperables Metadaten-Framework, das die Beschreibung von Geodaten mit zentralen Metainformationen wie räumlicher und zeitlicher Ausdehnung sowie technischen Details ermöglicht. Dadurch wird das Durchsuchen, Zugreifen und Austauschen von Geodaten verschiedener Anbieter über standardisierte Kataloge und APIs sowohl dynamisch als auch statisch erleichtert. Somit dient STAC der besseren Auffindbarkeit, Zugänglichkeit und Interoperabilität von Geodaten. STAC ist flexibel erweiterbar für diverse Anwendungsfälle und Datenformate, beispielsweise Satellitenbilder, Punktwolken oder Wetterdaten.

Hauptmerkmale
^^^^^^^^^^^^^

- **Datenmodell:** STAC definiert Objekte wie Item, Collection und Catalog, die Metadaten zu Geodaten enthalten. Diese Metadaten umfassen die räumliche und zeitliche Ausdehnung, technische Informationen, Lizenzbedingungen und mehr.
- **Format:** Die Daten werden häufig im GeoJSON-Format bereitgestellt, das eine einfache Integration in moderne GIS-Systeme ermöglicht.
- **API:** Die STAC API ermöglicht das Filtern und Abrufen von Geodaten basierend auf räumlichen, zeitlichen oder attributiven Eigenschaften. Dies erleichtert sowohl automatische als auch manuelle Suchvorgänge.
- **Interoperabilität:** STAC ist so konzipiert, dass es mit verschiedenen Werkzeugen wie QGIS und ArcGIS sowie mit Cloud-Speichern zusammenarbeitet. Es unterstützt die Visualisierung und Analyse von Geodaten.

Vorteile
^^^^^^^^
- **Standardisierung:** Einheitliche Struktur für Geodatenkataloge, die die Nutzung und Integration vereinfacht.
- **Flexibilität:** Raum für Erweiterungen, um spezifische Anforderungen abzudecken.
- **Effizienz:** Ermöglicht gezielte Abfragen nach Metainformationen wie Bounding Box oder Zeitstempel.

.. note:: STAC kommt zunehmend in Geodateninfrastrukturen zum Einsatz, beispielsweise bei der Bereitstellung freier Geodaten durch Behörden wie das Landesamt für Geoinformation Niedersachsen (LGLN).

FOSSGIS Konferenz 2024: `Bereitstellung von freien Geodaten (OpenData) mit STAC beim LGLN <https://youtu.be/m9ulOVSp6Rg?si=nb9nILfYS5NMGuKS>`_

----------------------------------------------------------------------------------------------

OpenData
--------







