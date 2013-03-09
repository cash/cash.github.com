Views
========
Elgg follows a MVC pattern and Views are the V in MVC. Views are responsible for creating the output. Generally, this will be HTML sent to a web browser, but it could also be RSS, JSON or any number of other data formats.

The Views system handles everything from the layout of pages and chunks of presentation output (like a footer or a toolbar) down to individual links and form inputs. It also allows for advanced features like automatic RSS generation, a swift-to-develop mobile interface, and the alternative interfaces suggested below. 

At their most basic level, the default views are just PHP files with snippets of html. For example::

   <h1>Hello, World!</h1>

Assuming this view is located at /views/default/hello.php, we could output it like so::

   echo elgg_view('hello');

For your convenience, Elgg comes with quite a lot of views by default. In order to keep things manageable, they are organized into subdirectories. Elgg handles this situation quite nicely. For example, our simple view might live in /views/default/hello/world.php, in which case it would be called like so::

   echo elgg_view('hello/world');

Well that's easy enough to remember! The name of the view simply reflects the location of the view in the views directory.

.. DANGER::
   Beware killer rabbits!

.. _test:

View an entity
-----------------

To view an entity, use elgg_view_entity().

