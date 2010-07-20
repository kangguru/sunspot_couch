Sunspot Couch
=============

Sunspot Rails provides Sunspot Adapters for CouchDB when also using Simply Stored

Usage
=====

copy the sunspot_couch.rb to somewhere from where it can be loaded

add these two lines to your sunspot.rb (or whatever file configures your sunspot)

  Sunspot::Adapters::InstanceAdapter.register(Sunspot::Couch::Adapters::CouchInstanceAdapter, SimplyStored::Couch)
  Sunspot::Adapters::DataAccessor.register(Sunspot::Couch::Adapters::CouchDataAccessor, SimplyStored::Couch)
  
for searchable-Support include "Sunspot::Rails::Searchable" within your model.
