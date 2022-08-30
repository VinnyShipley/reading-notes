# DRF Permissions

Requests Determine whether a request should be granted or denied. The simplest kind of permission would be to allow any authenticated user to make a request.

## How Permissions are Determined

Permissions in a REST framework are always defined as a list of permission classes. Before running the main body view of any page, a permission check will be rub, raising an exception error if it fails.

## Object Level Permissions

Not just for views, permissions can also be designated whether certain users have the ability to act on certain objects, which will usually be a model instance.

## Setting Permission Policies

The default permissions class may be set globally using the DEFAULT_PERMISSION_CLASSES setting, found in the settings file of the django app.

API permissions reference:

* AllowAny: will allow unrestricted access, regardless of if the request was authenticated or not.

* IsAuthenticated: will deny permission to any un-authenticated users

* IsAdminUser: will deny access unless the user.is_staff is True, in which case the permission will be cleared.

* IsAuthenticatedOrReadOnly: authenticated users can make any request, while unauthenticated users can only perform GET, HEAD, or OPTIONS


