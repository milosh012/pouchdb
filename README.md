Sync Multiple AngularJS Apps Without Server via PouchDB
=======================================================


This is a simple example from [this](http://mircozeiss.com/sync-multiple-angularjs-apps-without-server-via-pouchdb/) blog post. Thanks to the @zeMirco!

Here is used AngularJS and PouchDB to build a small app that syncs serverless and stores data persistently. Changes are distributed automatically. They can be made inside the database, on any client or on any third party device that pushes changes to the connected CouchDB. AngularJS events update our models in the controller that pushes changes to our views via two-way data binding. It is possible to add todos to the app when offline and as soon you are back online.

## Instalation:

1. Install [CouchDB](http://couchdb.apache.org)
2. Enable [CORS](http://docs.couchdb.org/en/latest/cors.html) in CouchDB (go to section httpd and set enable_cors to true)
3. Navigate to the bottom of the page and click on Add a new section
```
section: cors;
option: origins;
value: *
```
4. Create a new db "ng-db"

