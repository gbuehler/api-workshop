# QGIS Usage with OGC APIs

QGIS is a powerful open-source desktop GIS that natively supports OGC API standards. Here’s a simple step-by-step guide to **add and visualize OGC API - Features** and **OGC API - Maps** data in QGIS.

---

## 🚀 Step 1: Launch QGIS

Open **QGIS Desktop** (version 3.22 or higher recommended) on your computer.

---

## 🌐 Step 2: Add OGC API - Features as a Vector Layer

1. **Open Data Source Manager**: Click the “Open Data Source Manager” button or go to `Layer` > `Add Layer` > `Add Vector Layer`.
2. **Select “Protocol”**: In the left panel, click on the “Protocol” tab.
3. **Enter URL**: 
   - For example, use the **Daraa** demo endpoint:
     ```
     https://demo.ldproxy.net/daraa/collections/AeronauticCrv/items?f=json
     ```
   - This URL returns a GeoJSON of aeronautical curves in the Daraa dataset.
4. **Set Layer Name**: Optionally, set a layer name (e.g., `Daraa AeronauticCrv`).
5. **Click “Add”**: The layer will be loaded and displayed on your map canvas.

---

## 🗺️ Step 3: Add OGC API - Maps as a Raster Layer (Tiled Map)

1. **Open Browser Panel**: If not visible, go to `View` > `Panels` > `Browser Panel`.
2. **Add a WMS/WMTS Connection**:
   - Right-click on “WMS/WMTS” and select “New Connection…”.
   - **Name**: e.g., `OGC API Maps`.
   - **URL**: Many OGC API - Maps endpoints also support WMS-like access. Use a compatible URL.
   - Example: 
     ```
     https://demo.ldproxy.net/daraa/tiles/WorldCRS84Quad/1.0.0/daraa/default/0/0/0
     ```
     (Adjust to the actual OGC API - Maps endpoint you want to explore.)
3. **Click “OK”**.
4. **Add the Layer**: Double-click the new connection and drag the layer to the map canvas.

---

## 🔍 Step 4: Explore the Data

- **Layer Styling**: Use the “Layer Styling” panel to adjust colors, symbols, and labels for better visualization.
- **Attribute Table**: Right-click the vector layer and choose “Open Attribute Table” to inspect feature attributes.
- **Spatial Queries**: Use tools like “Select by Location” to perform spatial queries with your data.

---

## 📝 Notes

- QGIS can connect to **any OGC API - Features** endpoint that provides GeoJSON, GML, or other supported vector data formats.
- For **time-enabled datasets** (like weather radar from the Meteorological Service of Canada), explore time-series animation in QGIS via the **Temporal Controller**.

---

## 💡 Additional Links

- QGIS Documentation: [https://docs.qgis.org/latest/en/docs/user_manual/](https://docs.qgis.org/latest/en/docs/user_manual/)
- OGC API - Features: [https://ogcapi.ogc.org/features/overview.html](https://ogcapi.ogc.org/features/overview.html)

---

By following these steps, workshop participants will see **how QGIS integrates with OGC APIs**, offering a powerful desktop environment to work with modern geospatial standards!

