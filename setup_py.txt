import setuptools

with open("README.md", "r", encoding="utf-8") as f:
    LONG_DESC = f.read()


__version__ = "0.0.0"

REPO_NAME = "kidney_kaggle"
AUTHOR_USER_NAME = "subhajit-dubey"
SRC_REPO = "cnn_kidney"
AUTHOR_EMAIL = "subhajit.dubey@gmail.com"
DESC = "A small Python package for CNN app"


setuptools.setup(
    name=SRC_REPO,
    version=__version__,
    author=AUTHOR_USER_NAME,
    author_email=AUTHOR_EMAIL,
    description=DESC,
    long_description=LONG_DESC,
    long_description_content="text/markdown",
    url=f"https://github.com/{AUTHOR_USER_NAME}/{REPO_NAME}",
    project_urls={
        "Bug Tracker": f"https://github.com/{AUTHOR_USER_NAME}/{REPO_NAME}/issues",
    },
    package_dir={"": "src"},
    packages=setuptools.find_packages(where="src")
)