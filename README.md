 
---
license: cc-by-nc-4.0

language:
- en # Language of the dataset card description

pretty_name: "Hieroglyphic Layout Analysis (HLA) Dataset"
tags:
- hieroglyphs
- ancient-egyptian
- image-segmentation
- layout-analysis
- computer-vision
- historical-documents
- archaeology
task_categories:
- image-segmentation
- object-detection # Identifying lines and cartouches can also be considered object detection

---

# Ancient Egyptian Hieroglyphic Datasets

## Datasets for Ancient Egyptian Hieroglyphic Research

### Hieroglyphic Layout Analysis (HLA) Dataset

**Overview:** The Hieroglyphic Layout Analysis (HLA) Dataset is a unique resource comprising **897 high-resolution images**, each containing multiple lines of Ancient Egyptian hieroglyphs and cartouches. This dataset is specifically designed for tasks related to identifying and segmenting the layout of hieroglyphic texts within artifact images.

**Data Collection:** The HLA Dataset was meticulously compiled from diverse sources:

* **Direct Collection (Egyptian Museum in Cairo, Egypt):** During on-site visits, we captured **230 high-resolution images** of various artifacts, including Pharaonic coffins, statues, and wall inscriptions housed in the Egyptian Museum in Cairo.
* **Online Museum Repositories:** We leveraged the growing trend of museums providing open access to their collections, gathering over **300 images** from **The Metropolitan Museum of Art (“The Met”), New York, USA**. The Met’s extensive collection spans approximately 30,000 objects of artistic, historical, and cultural significance, dating from around 300,000 BCE to the 4th century CE.
* **Museo Egizio, Turin, Italy:** We also collected more than **200 images** from the **Egyptian Museum in Turin (“Museo Egizio”)**, which has made over 4,000 of its approximately 40,000 objects accessible online.
* **Specific Archaeological Sites:** The dataset includes **18 images** of the wall inscriptions within the **Unas pyramid in Giza, Egypt**, known for their dense concentration of hieroglyphic signs.
* **Additional Online Resources:** Further images were sourced from the online collections of:
    * The French Institute for Oriental Archaeology (IFAO) in Cairo
    * The Rosicrucian Egyptian Museum (REM), USA
    * The British Museum, UK
    * The Museum of Fine Arts in Boston, USA
    * The Louvre Museum in Paris
    * The Egyptian Museum and Papyrus Collection of Berlin, Germany
    * General online searches for relevant artifacts.

**Annotation Details:** Following image collection and rigorous selection, every instance within the HLA Dataset underwent manual segmentation and annotation using the CVAT platform. Polygonal segmentation masks were created for two primary classes: **“Line”** (representing rows of hieroglyphs) and **“Cartouche”** (oval enclosures containing royal names). Individual images within the dataset can contain a significant number of these objects, with some images featuring up to **152 distinct lines or cartouches**.

**Key Statistics:**
* **Total Images:** 897
* **Annotation Classes:** 2 (“Line”, “Cartouche”)
* **Annotation Type:** Polygon Segmentation Masks
* **Maximum Objects per Image:** 152

**Potential Uses:** This dataset is ideal for training and evaluating models for:
* Hieroglyphic line detection and segmentation.
* Cartouche detection and segmentation.
* Layout analysis of hieroglyphic inscriptions on various artifact types.

**Json annotation files "in coco format":**
* Train: 705 images.
* Validation: 178 images.
* Test: 10 images.