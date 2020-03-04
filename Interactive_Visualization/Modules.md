## Visualization packages

Overview: https://pyviz.org/overviews/index.html

**Matplotlib** is a Python 2D plotting library which produces publication quality figures in a variety of hardcopy formats and interactive environments across platforms.

The output of a jupyter notebook cell gives:
```
"outputs": [
    {
     "data": {
      "image/png": "iVBORw0KGgoAAAANSUhEUgAAAwEAAAFNCAYAAABYGmMrAAAABHNCSVQICAgIfAhkiAAAAAlwSFlzAAALEgAACxIB0t1+/AAAADl0RVh
0U29mdHdhcmUAbWF0cGxvdGxpYiB2ZXJzaW9uIDMuMC4yLCBodHRwOi8vbWF0cGxvdGxpYi5vcmcvOIA7rQAAIABJREFUeJzs3XecFdX9//HXBxBWAcGGDQOoqF
gCAUSNbTXR2PGr8RdLItEk2I0xiSUmsSeamK+ab4qa2Hs3xpiCZTXYEBQbWBEVRUCauwLLLvv5/TFn4e7l3t2Zu3dvfT8fj91775QzZ87MnDln5pwZc3dERERER
KR6dCt2BEREREREpLBUCRARERERqTKqBIiIiIiIVBl .....
```
**Creating and displaying images like Pngs, jpgs etc are not efficient.**


## Bokeh

is an interactive visualization library that targets modern web browsers for presentation

https://bokeh.pydata.org/en/latest/

## Let's have a look at the output cells

* importing the library introduces new Js functions

```
 "outputs": [
    {
     "data": {
      "application/javascript": [
       "\n",
       "(function(root) {\n",
       "  function now() {\n",
       "    return new Date();\n",
       "  }\n",
       "\n",
       "  var force = true;\n",
       "\n",
```

* The outputs are javascript codes, that contain html and css as well:

```
"outputs": [
    {
     "data": {
      "application/javascript": [
       "// Ugly hack - see HoloViews #2574 for more information\n",
       "if (!(document.getElementById('1734')) && !(document.getElementById('_anim_img1734'))) {\n",
       "  console.log(\"Creating DOM nodes dynamically for assumed nbconvert export. To generate clean HTML output set HV_D
OC_HTML as an environment variable.\")\n",
       "  var htmlObject = document.createElement('div');\n",
       "  htmlObject.innerHTML =
       "  <div class=\"bk-root\" id=\"d70afa8e-dad5-447b-86dd-dc6647948442\" data-root-id=\"1734\"></div>\n",
       "`;\n",
       "  var scriptTags = document.getElementsByTagName('script');\n",.....
```

### Creating interactive Dashboards

* Bokeh server
* Plotly dash server
* Pyviz.org
* Holoviews
