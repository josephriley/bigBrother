# bigBrother
Authority Identification TensorFlow Model.

Identifies Police, Firefighter, EMS, & Civilians.

## Example

You will need Python 3.6 and the path to an image.

Create a virtual environment

`python -m venv tf-venv`

Activate the virtual environment

macOS `source tf-venv/bin/activate`

Windows `tf-venv/Scripts/activate`

Install the the dependencies for the example

`python -m pip install --upgrade pip && pip install -r requirements.txt`

Run the example and see the model output

`python tf_example.py path/to/image/for/testing`

### Note:

If you see the error "OSError: image file is truncated", you may need to add the following to the sample code due to an issue with PIL (Python Image Library)

```python
from PIL import ImageFile
ImageFile.LOAD_TRUNCATED_IMAGES = True
```

## License

This project is made available under the MIT license. See the LICENSE file for more information.
