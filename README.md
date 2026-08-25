# GeoAI in Practice: From Geospatial Data to Graph Neural Networks with City2Graph

<p align="center"><img src="img/workshop_thumbnail.jpg" width="600" alt="Workshop Thumbnail"></p>

> **Both FOSS4G 2026 submissions have been accepted and are included in the final programme.**
>
> | Track | Session | Schedule |
> | --- | --- | --- |
> | Workshop | [**GeoAI in Practice: From Geospatial Data to Graph Neural Networks with City2Graph**](https://talks.osgeo.org/foss4g-2026-workshop/talk/ZPM3WY/) | 31 August 2026, 14:00–17:00, Room 609 |
> | General track | [**City2Graph: Open Source Python Library for GeoAI with Graph Neural Networks**](https://talks.osgeo.org/foss4g-2026/talk/LV8FCQ/) | 1 September 2026, 16:00–16:30, Room 4 |

## Content

This workshop introduces Graph Neural Networks (GNNs) for geospatial practitioners. Using open-source Python tools including PyTorch Geometric and [City2Graph](https://github.com/c2g-dev/city2graph), participants will learn how to transform urban geospatial data into network structures and apply GNNs to model complex spatial relations.

**Part 1: Graph Data Engineering, Spatial Network Analysis, and GNNs** [Jupyter Notebook](notebooks/part1_networks.ipynb)

Learn to construct and analyse spatial networks using GeoPandas and NetworkX. We will demonstrate how to convert standard geospatial data (e.g., OpenStreetMap, GTFS, etc.) into unified graph structures with OSMnx and City2Graph. We will then explore key GNN architectures and transition from spatial graphs into tensor formats using PyTorch Geometric and City2Graph.

**Part 2: Build Your Own GeoAI Pipeline** [Jupyter Notebook](notebooks/part2_geoai.ipynb)

Put your skills into practice. Choose a city, extract its street network from OpenStreetMap or Overture Maps (optional), and train a Graph Autoencoder (GAE) for an unsupervised spatial clustering task. We will conclude by discussing how the GNN pipeline could be adopted for your business / research workflows.

Google Colab is also available:

Part 1:
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1aGeFnTPv83A8oN4UES2IZ424XceSRi13)

Part 2:
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1MKnc8nG0oGKTZIy_ZTQLTsUl9vez94Jz)

## Quickstart

### Option 1: Local Environment

This repository uses [uv](https://docs.astral.sh/uv/) for environment and dependency management.

I. Install dependencies and create the local virtual environment:

```bash
uv sync
```

II. Start Jupyter Notebook using either of these options:

Option A: run Jupyter directly with `uv`:

```bash
uv run jupyter notebook
```

Option B: activate the virtual environment in your editor terminal, then launch Jupyter:

```bash
source .venv/bin/activate
jupyter notebook
```

III. Open [notebooks/part1_networks.ipynb](notebooks/part1_networks.ipynb) (Part 1) and [notebooks/part2_geoai.ipynb](notebooks/part2_geoai.ipynb) (Part 2) in Jupyter Notebook.

Python `>=3.11,<3.14` is required. If `uv` is not installed yet, see the [uv installation guide](https://docs.astral.sh/uv/getting-started/installation/).

### Option 2: Google Colab

If you are using Google Colab, you need to have a Google account. The Colab link provided above is in viewer mode, so please save a copy to your own Google Drive (`File > Save a copy in Drive`) before running the notebook.

## Who is this for?
* **Target Audience:** GIS analysts, spatial data scientists, and Python developers expanding their GeoAI and network modelling skills.

* **Prerequisites:** Basic proficiency in Python (especially GeoPandas) and GIS concepts. Basic knowledge of machine learning and neural networks (e.g., supervised vs. unsupervised learning, loss functions, activation functions, backpropagation). If you are not familiar with those topics of neural networks, I recommend watching 3Blue1Brown’s tutorial videos (Chapter 1-4) in advance ([English](https://www.youtube.com/playlist?list=PLZHQObOWTQDNU6R1_67000Dx_ZCJB-3pi) [Español](https://www.youtube.com/playlist?list=PLIb_io8a5NB0CP5ktJE9qaLd6GOfh1Z9m) [한국어](https://www.youtube.com/watch?v=wrguEHxk_EI&list=PLkoaXOTFHiqhM4MeCMrS016jOWKfIXTjK&index=6) [हिंदी](https://www.youtube.com/watch?v=uiZL9rK2Q_Q&list=PLxGL0qHs2IM0eZxOcYROIBd11XVKiyTeg) [日本語](https://www.youtube.com/watch?v=tc8RTtwvd5U) [русский](https://www.youtube.com/watch?v=RJCIYBAAiEI&list=PLZjXXN70PH5itkSPe6LTS-yPyl5soOovc) [中文](https://space.bilibili.com/88461692/lists/1528929?type=series)). No prior network science (NetworkX) or GNN (PyTorch Geometric) skills required.

## Data sources and licences

* **OpenStreetMap:** Data © [OpenStreetMap contributors](https://www.openstreetmap.org/copyright), available under the Open Database License (ODbL).

* **Overture Maps:** Transportation data © OpenStreetMap contributors, [Overture Maps Foundation](https://overturemaps.org/), available under the ODbL. See the [Overture Maps attribution and licensing guidance](https://docs.overturemaps.org/attribution/).

* **Hiroden GTFS:** GTFS data published through the [Hiroshima Bus Association](https://www.bus-kyo.or.jp/gtfs-open-data), available under CC0.

Third-party datasets remain governed by their respective licences.

## News
* **2026-08-25:** Part 1 was expanded with materials on Overture Maps, GTFS transit graphs, spatial graph construction, and GNNs. Updated Jupyter Notebook and Google Colab versions are now available.

* **2026-03-08:** Repository updated for the upcoming workshop in **FOSS4G 2026 Hiroshima**.
