==================
PyAMS chat package
==================

.. contents::


What is PyAMS?
==============

PyAMS (Pyramid Application Management Suite) is a small suite of packages written for applications
and content management with the Pyramid framework.

**PyAMS** is actually mainly used to manage web sites through content management applications (CMS,
see PyAMS_content package), but many features are generic and can be used inside any kind of web
application.

All PyAMS documentation is available on `ReadTheDocs <https://pyams.readthedocs.io>`_; source code
is available on `Gitlab <https://gitlab.com/pyams>`_ and pushed to `Github
<https://github.com/py-ams>`_. Doctests are available in the *doctests* source folder.


What is PyAMS chat?
===================

PyAMS_chat is a small package used to communicate with PyAMS_chat_ws package, which can be used
to send notifications to connected users using websockets.

PyAMS_chat relies on a Redis server on which notifications are published; a *pubsub* listener is
then used by PyAMS_chat_ws server to receive published messages and dispatch them on connected
users.
