
====================
Blick in die Zukunft
====================

**Datenbereitstellung über Geodatendienste oder Schnittstellen (API)**

In Zukunft werden die bestehenden Standards durch neue Standards, d.h. Geodatendienste durch Schnittstellen ergänzt oder ersetzt. Hier werden die wichtigsten APIs beschrieben, die sich derzeit in der Entwicklung befinden.

----------------------------------------------------------------------------------------------

OGC APIs
--------

Die OGC APIs sind eine Familie von Standards, die vom `Open Geospatial Consortium (OGC) <https://ogcapi.ogc.org/#standards>`_ entwickelt wurden, um den Zugang und die Nutzung von Geodaten über das Web zu vereinfachen und zu standardisieren. Diese APIs sind modular aufgebaut und definieren wiederverwendbare Bausteine für raumbezogene Web-APIs.


Hauptmerkmale
"""""""""""""

- **Standardisierung:** OGC APIs folgen einer einheitlichen Struktur, die auf Web-Standards wie HTTP und OpenAPI basiert.
- **Modularität:** Die Standards sind in verschiedene Teile gegliedert, die jeweils spezifische Funktionen abdecken.
- **Interoperabilität:** Sie ermöglichen eine konsistente Interaktion mit Geodaten über verschiedene Systeme hinweg.


Kernfunktionen
""""""""""""""

- **Datenzugriff:** OGC APIs ermöglichen das Abrufen, Erstellen und Ändern von Geodaten.
- **Abfragemöglichkeiten:** Sie bieten Funktionen zum Filtern und Abfragen von Daten.
- **Formatunterstützung:** Antworten werden typischerweise in JSON oder HTML geliefert.

.. note:: OGC APIs sind eine Weiterentwicklung älterer Standards und sollen die Integration von Geodaten in moderne Anwendungen erleichtern.


---------------------------------------------------------------------------------------------


Welche APIs ersetzen welche Standards?
----------------------------------------


OGC API - Records
"""""""""""""""""

Die OGC API - Records soll den Catalogue Service for the Web (CSW) ersetzen und dient der Suche und Abfrage von Metadaten.


OGC API - Features
""""""""""""""""""

Die OGC API - Features ersetzt den Web Feature Service (WFS). Sie ermöglicht das Erstellen, Ändern und Abfragen von räumlichen Daten im Web.

.. note:: Einige Länder haben bereits OGC-API - Features veröffentlicht (z.B. RP, NRW, SL, HH), wobei sich die APIs in ihrer Struktur unterscheiden. Einige APIs bieten einen direkten Datendownload an (z.B. RP, SL), andere sind kaskadierend aufgebaut (HH), hier gelangt man beim Aufruf der API auf eine Landingpage, auf der die Daten zum Download angeboten werden. Aus diesem Grund werden in der Suche weniger Treffer angezeigt.


OGC API - Maps
""""""""""""""

Die OGC API - Maps soll den Web Map Service (WMS) ersetzen. Sie ermöglicht die Darstellung von digitalen Karten in Kartenviewern.


OGC API - Tiles
"""""""""""""""

Die OGC API - Tiles ist der Nachfolger des Web Map Tile Service (WMTS). Sie unterstützt verschiedene Formen gekachelter Geodaten, einschließlich Vektorkacheln, Karten und Bilder.

----------------------------------------------------------------------------------------------

STAC-Standard / STAC API
------------------------

Der STAC-Standard (SpatioTemporal Asset Catalog) ist ein offener Standard für die Beschreibung, Katalogisierung und Abfrage von Geodaten. Er wurde entwickelt, um den Zugang zu raum-zeitlichen Daten wie Bilddaten, Punktwolken oder digitalen Orthophotos zu vereinfachen und zu standardisieren.

Hauptmerkmale
"""""""""""""

- **Datenmodell:** STAC definiert Objekte wie Item, Collection und Catalog, die Metadaten zu Geodaten enthalten. Diese Metadaten umfassen die räumliche und zeitliche Ausdehnung, technische Informationen, Lizenzbedingungen und mehr.
- **Format:** Die Daten werden häufig im GeoJSON-Format bereitgestellt, das eine einfache Integration in moderne GIS-Systeme ermöglicht.
- **API:** Die STAC API ermöglicht das Filtern und Abrufen von Geodaten basierend auf räumlichen, zeitlichen oder attributiven Eigenschaften. Dies erleichtert sowohl automatische als auch manuelle Suchvorgänge.
- **Interoperabilität:** STAC ist so konzipiert, dass es mit verschiedenen Werkzeugen wie QGIS und ArcGIS sowie mit Cloud-Speichern zusammenarbeitet. Es unterstützt die Visualisierung und Analyse von Geodaten.

Vorteile
""""""""
- **Standardisierung:** Einheitliche Struktur für Geodatenkataloge, die die Nutzung und Integration vereinfacht.
- **Flexibilität:** Raum für Erweiterungen, um spezifische Anforderungen abzudecken.
- **Effizienz:** Ermöglicht gezielte Abfragen nach Metainformationen wie Bounding Box oder Zeitstempel.

.. note:: STAC wird zunehmend in Geodateninfrastrukturen eingesetzt, z.B. bei der Bereitstellung von freien Geodaten durch Behörden wie das Landesamt für Geoinformation Niedersachsen (LGLN).

----------------------------------------------------------------------------------------------
