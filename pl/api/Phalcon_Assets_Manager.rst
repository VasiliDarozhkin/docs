Class **Phalcon\\Assets\\Manager**
==================================

Manages collections of CSS/Javascript assets


Methods
-------

public  **__construct** ([*array* $options])





public  **setOptions** (*unknown* $options)

Sets the manager options



public  **getOptions** ()

Returns the manager options



public  **useImplicitOutput** (*unknown* $implicitOutput)

Sets if the HTML generated must be directly printed or returned



public  **addCss** (*unknown* $path, [*unknown* $local], [*unknown* $filter], [*unknown* $attributes])

Adds a Css resource to the 'css' collection 

.. code-block:: php

    <?php

    $assets->addCss('css/bootstrap.css');
    $assets->addCss('http://bootstrap.my-cdn.com/style.css', false);




public  **addInlineCss** (*unknown* $content, [*unknown* $filter], [*unknown* $attributes])

Adds a inline Css to the 'css' collection



public  **addJs** (*unknown* $path, [*unknown* $local], [*unknown* $filter], [*unknown* $attributes])

Adds a javascript resource to the 'js' collection 

.. code-block:: php

    <?php

    $assets->addJs('scripts/jquery.js');
    $assets->addJs('http://jquery.my-cdn.com/jquery.js', false);




public  **addInlineJs** (*unknown* $content, [*unknown* $filter], [*unknown* $attributes])

Adds a inline javascript to the 'js' collection



public  **addResourceByType** (*unknown* $type, *unknown* $resource)

Adds a resource by its type 

.. code-block:: php

    <?php

    $assets->addResourceByType('css', new \Phalcon\Assets\Resource\Css('css/style.css'));




public  **addInlineCodeByType** (*unknown* $type, *unknown* $code)

Adds a inline code by its type



public  **addResource** (*unknown* $resource)

Adds a raw resource to the manager 

.. code-block:: php

    <?php

     $assets->addResource(new Phalcon\Assets\Resource('css', 'css/style.css'));




public  **addInlineCode** (*unknown* $code)

Adds a raw inline code to the manager



public  **set** (*unknown* $id, *unknown* $collection)

Sets a collection in the Assets Manager 

.. code-block:: php

    <?php

     $assets->set('js', $collection);




public  **get** (*unknown* $id)

Returns a collection by its id 

.. code-block:: php

    <?php

     $scripts = $assets->get('js');




public  **getCss** ()

Returns the CSS collection of assets



public  **getJs** ()

Returns the CSS collection of assets



public  **collection** (*unknown* $name)

Creates/Returns a collection of resources



public  **output** (:doc:`Phalcon\\Assets\\Collection <Phalcon_Assets_Collection>` $collection, *callback* $callback, *string* $type)

Traverses a collection calling the callback to generate its HTML



public  **outputInline** (:doc:`Phalcon\\Assets\\Collection <Phalcon_Assets_Collection>` $collection, *string* $type)

Traverses a collection and generate its HTML



public  **outputCss** ([*string* $collectionName])

Prints the HTML for CSS resources



public  **outputInlineCss** ([*string* $collectionName])

Prints the HTML for inline CSS



public  **outputJs** ([*string* $collectionName])

Prints the HTML for JS resources



public  **outputInlineJs** ([*string* $collectionName])

Prints the HTML for inline JS



public  **getCollections** ()

Returns existing collections in the manager



