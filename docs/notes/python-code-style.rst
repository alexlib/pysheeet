=====
Style
=====

.. contents:: Table of Contents
    :backlinks: none

Naming
------

Class
^^^^^

Bad

.. code-block:: python

    class fooClass: ...
    class foo_class: ...

Good

.. code-block:: python

    class FooClass: ...


Function
^^^^^^^^

Bad

.. code-block:: python

    def CapCamelCase(*a): ...
    def mixCamelCase(*a): ...

Good

.. code-block:: python

    def func_separated_by_underscores(*a): ...

Variable
^^^^^^^^

Bad

.. code-block:: python

    FooVar = "CapWords"
    fooVar = "mixedCase"
    Foo_Var = "CapWords_With_Underscore"

Good

.. code-block:: python

    # local variable
    var = "lowercase"

    # internal use
    _var = "_single_leading_underscore"

    # avoid conflicts with Python keyword
    var_ = "single_trailing_underscore_"

    # a class attribute (private use in class)
<<<<<<< HEAD
    var = " __double_leading_underscore"
=======
    __var = " __double_leading_underscore"
>>>>>>> 5250bd678d7615ad45acec05da327ab93a387e9d

    # "magic" objects or attributes, ex: __init__
    __name__

    # throwaway variable, ex: _, v = (1, 2)
    _ = "throwaway"
