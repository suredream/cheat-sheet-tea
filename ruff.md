
__Install__

    pip install ruff

__Config__

    %%writefile ruff.toml
    # Enable pycodestyle (`E`) and Pyflakes (`F`) codes by default.
    select = ["E", "F"]
    ignore = ["E501","E401"]

    target-version = "py38"

__autofix__

    !ruff check smb/core.py --fix