# Gimpimagelevel

[Gimpformats Index](../README.md#gimpformats-index) / [Gimpformats](./index.md#gimpformats) / Gimpimagelevel

> Auto-generated documentation for [gimpformats.GimpImageLevel](../../../gimpformats/GimpImageLevel.py) module.

- [Gimpimagelevel](#gimpimagelevel)
  - [GimpImageLevel](#gimpimagelevel)
    - [GimpImageLevel().__repr__](#gimpimagelevel()__repr__)
    - [GimpImageLevel().__str__](#gimpimagelevel()__str__)
    - [GimpImageLevel()._encodeRLE](#gimpimagelevel()_encoderle)
    - [GimpImageLevel()._imgToTiles](#gimpimagelevel()_imgtotiles)
    - [GimpImageLevel().bpp](#gimpimagelevel()bpp)
    - [GimpImageLevel().decode](#gimpimagelevel()decode)
    - [GimpImageLevel().encode](#gimpimagelevel()encode)
    - [GimpImageLevel().image](#gimpimagelevel()image)
    - [GimpImageLevel().image](#gimpimagelevel()image-1)
    - [GimpImageLevel().mode](#gimpimagelevel()mode)
    - [GimpImageLevel().tiles](#gimpimagelevel()tiles)

## GimpImageLevel

[Show source in GimpImageLevel.py:19](../../../gimpformats/GimpImageLevel.py#L19)

Gets packed pixels from a gimp image.

This represents a single level in an imageHierarchy

#### Signature

```python
class GimpImageLevel(GimpIOBase):
    def __init__(self, parent) -> None: ...
```

#### See also

- [GimpIOBase](./GimpIOBase.md#gimpiobase)

### GimpImageLevel().__repr__

[Show source in GimpImageLevel.py:284](../../../gimpformats/GimpImageLevel.py#L284)

Get a textual representation of this object.

#### Signature

```python
def __repr__(self, indent: int = 0) -> str: ...
```

### GimpImageLevel().__str__

[Show source in GimpImageLevel.py:280](../../../gimpformats/GimpImageLevel.py#L280)

Get a textual representation of this object.

#### Signature

```python
def __str__(self) -> str: ...
```

### GimpImageLevel()._encodeRLE

[Show source in GimpImageLevel.py:150](../../../gimpformats/GimpImageLevel.py#L150)

Encode image to RLE image data.

#### Signature

```python
def _encodeRLE(self, data, bpp): ...
```

### GimpImageLevel()._imgToTiles

[Show source in GimpImageLevel.py:245](../../../gimpformats/GimpImageLevel.py#L245)

break an image into a series of tiles, each<=64x64.

#### Signature

```python
def _imgToTiles(self, image): ...
```

### GimpImageLevel().bpp

[Show source in GimpImageLevel.py:225](../../../gimpformats/GimpImageLevel.py#L225)

Get bpp.

#### Signature

```python
@property
def bpp(self): ...
```

### GimpImageLevel().decode

[Show source in GimpImageLevel.py:32](../../../gimpformats/GimpImageLevel.py#L32)

Decode a byte buffer.

#### Arguments

- `data` - data buffer to decode
- `index` - index within the buffer to start at

#### Signature

```python
def decode(self, data: bytes, index: int = 0) -> int: ...
```

### GimpImageLevel().encode

[Show source in GimpImageLevel.py:72](../../../gimpformats/GimpImageLevel.py#L72)

Encode this object to a byte buffer.

#### Signature

```python
def encode(self) -> bytearray: ...
```

### GimpImageLevel().image

[Show source in GimpImageLevel.py:256](../../../gimpformats/GimpImageLevel.py#L256)

Get a final, compiled image.

#### Signature

```python
@property
def image(self) -> Image: ...
```

### GimpImageLevel().image

[Show source in GimpImageLevel.py:272](../../../gimpformats/GimpImageLevel.py#L272)

#### Signature

```python
@image.setter
def image(self, image: Image) -> None: ...
```

### GimpImageLevel().mode

[Show source in GimpImageLevel.py:230](../../../gimpformats/GimpImageLevel.py#L230)

Get mode.

#### Signature

```python
@property
def mode(self): ...
```

### GimpImageLevel().tiles

[Show source in GimpImageLevel.py:236](../../../gimpformats/GimpImageLevel.py#L236)

Get tiles.

#### Signature

```python
@property
def tiles(self): ...
```