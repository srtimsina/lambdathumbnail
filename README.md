# lambdathumbnail
To create package python function
``` bash
virtualenv labvenv
source labvenv/bin/activate
pip install Pillow
pip show Pillow
deactivate
cd labvenv/lib/python3.7/site-packages
zip -r deployment-package.zip .
mv deployment-package ~/
cd ~/
zip -g deployment-package.zip lambda_function.py
```
