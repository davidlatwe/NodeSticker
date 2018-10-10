<h1 align=center>NodeSticker</h1>

<p align=center><i>Put custom icon on any Maya node for display in the GUI.</i></p>

<p align=center><img src="https://user-images.githubusercontent.com/3357009/46756698-a6f89780-ccfa-11e8-8ded-d6602e9f9fff.gif"></p>

### Example

```python
from sticker import NodeSticker

sticker = NodeSticker()

# Set icon
sticker.set(["nodeShape1", "nodeShape2"], "polyCube.png")
sticker.set("nodeShape3", "path/to/my_icon.png")

# Revert to default
sticker.revert("nodeShape1")

# Reveal from saved file
sticker.show()

```

### Note
* Icon file format must be `PNG`.
* Preferred size in the Outliner is 20 x 20 pixels.
* File path can be an absolute path or be relative to the `XBMLANGPATH` environment variable.
* Will add a custom attribute `customIconPath` in node to save icon path.
* Powered by Maya Python API 1.0 (Can not achieve with 2.0)

