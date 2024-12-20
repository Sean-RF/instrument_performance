# Instrument Performance study


<!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->

Start by creating an object that will hold all of the parameters. This
can be patched to as neccesary. I haven’t decided if I want to implement
support for handling which variables are dependent/independent. For now,
I’m going to just compute things as in the GEMS CUBIC NASA AOS
Performance sheet.

``` python
instrument_parameters = {
    "alittude": 450e3, # geodetic orbital altitude in m
    "scan_angle_limit" : 45 # scan angle limit in degrees
}
```

------------------------------------------------------------------------

### Instrument

>  Instrument ()

*An instance of an instrument to be studied.*

------------------------------------------------------------------------

### Instrument.amethod

>  Instrument.amethod ()

*stuff will be computed*

------------------------------------------------------------------------

### Instrument.anothermethod

>  Instrument.anothermethod (x:float=0)

<table>
<thead>
<tr>
<th></th>
<th><strong>Type</strong></th>
<th><strong>Default</strong></th>
<th><strong>Details</strong></th>
</tr>
</thead>
<tbody>
<tr>
<td>x</td>
<td>float</td>
<td>0</td>
<td>x has special qualities</td>
</tr>
</tbody>
</table>

``` python
methlist = [method for method in dir(Instrument) if method.startswith('__') is False]
for method in methlist:
    showdoc.show_doc(getattr(Instrument,method))
```

``` python
#hide_input

showdoc.show_doc(getattr(Instrument,methlist[0]))
showdoc.show_doc(getattr(Instrument,methlist[1]))
```

------------------------------------------------------------------------

### Instrument.anothermethod

>  Instrument.anothermethod (x:float=0)

<table>
<thead>
<tr>
<th></th>
<th><strong>Type</strong></th>
<th><strong>Default</strong></th>
<th><strong>Details</strong></th>
</tr>
</thead>
<tbody>
<tr>
<td>x</td>
<td>float</td>
<td>0</td>
<td>x has special qualities</td>
</tr>
</tbody>
</table>

``` python
from numpy import all
showdoc.show_doc(all)
```

    /opt/hostedtoolcache/Python/3.12.8/x64/lib/python3.12/site-packages/fastcore/docscrape.py:230: UserWarning: Unknown section See Also
      else: warn(msg)

------------------------------------------------------------------------

### all

>  all (a, axis=None, out=None, keepdims=<no value>, where=<no value>)

*Test whether all array elements along a given axis evaluate to True.*

<table>
<colgroup>
<col style="width: 6%" />
<col style="width: 25%" />
<col style="width: 34%" />
<col style="width: 34%" />
</colgroup>
<thead>
<tr>
<th></th>
<th><strong>Type</strong></th>
<th><strong>Default</strong></th>
<th><strong>Details</strong></th>
</tr>
</thead>
<tbody>
<tr>
<td>a</td>
<td>array_like</td>
<td></td>
<td>Input array or object that can be converted to an array.</td>
</tr>
<tr>
<td>axis</td>
<td>NoneType</td>
<td>None</td>
<td>Axis or axes along which a logical AND reduction is
performed.<br>The default (<code>axis=None</code>) is to perform a
logical AND over all<br>the dimensions of the input array.
<code>axis</code> may be negative, in<br>which case it counts from the
last to the first axis. If this<br>is a tuple of ints, a reduction is
performed on multiple<br>axes, instead of a single axis or all the axes
as before.</td>
</tr>
<tr>
<td>out</td>
<td>NoneType</td>
<td>None</td>
<td>Alternate output array in which to place the result.<br>It must have
the same shape as the expected output and its<br>type is preserved
(e.g., if <code>dtype(out)</code> is float, the result<br>will consist
of 0.0’s and 1.0’s). See :ref:<code>ufuncs-output-type</code><br>for
more details.</td>
</tr>
<tr>
<td>keepdims</td>
<td>_NoValueType</td>
<td><no value></td>
<td>If this is set to True, the axes which are reduced are left<br>in
the result as dimensions with size one. With this option,<br>the result
will broadcast correctly against the input array.<br><br>If the default
value is passed, then <code>keepdims</code> will not be<br>passed
through to the <code>all</code> method of sub-classes
of<br><code>ndarray</code>, however any non-default value will be. If
the<br>sub-class’ method does not implement <code>keepdims</code>
any<br>exceptions will be raised.</td>
</tr>
<tr>
<td>where</td>
<td>_NoValueType</td>
<td><no value></td>
<td>Elements to include in checking for all <code>True</code>
values.<br>See <code>~numpy.ufunc.reduce</code> for details.<br><br>..
versionadded:: 1.20.0</td>
</tr>
<tr>
<td><strong>Returns</strong></td>
<td><strong>ndarray, bool</strong></td>
<td></td>
<td><strong>A new boolean or array is returned unless <code>out</code>
is specified,<br>in which case a reference to <code>out</code> is
returned.</strong></td>
</tr>
</tbody>
</table>