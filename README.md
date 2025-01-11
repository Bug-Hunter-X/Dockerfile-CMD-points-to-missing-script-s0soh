# Dockerfile Bug: Missing Script in CMD Instruction

This repository demonstrates a common error in Dockerfiles: the `CMD` instruction points to a script that's not included in the image.

The original `Dockerfile` attempts to run a Python script, `my_script.py`, but this script is missing from the image, leading to a runtime error.

The solution involves adding the application code (`my_script.py` and `requirements.txt`) to the image.