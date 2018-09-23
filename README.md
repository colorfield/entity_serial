# Entity Serial

Per bundle computed serial number for entities.

The difference with the
[Serial](https://www.drupal.org/project/serial) module 
is that the field value is not stored but computed.

The sequence is preserved if entities from the bundle
are being deleted.

### Use case

When a sequence within a bundle is needed (e.g. invoice number, ...).

### Configuration

Add the field to an entity type bundle (e.g. _Article_ content type).
Set the serial id to start from and the node id that will be used 
as the first entity to count from. 

### Roadmap

- Optionally initialize values for existing entities
- Lightweight system wide configuration without per bundle field definition by implementing
 _hook_entity_bundle_field_info()_ [WIP]

### Related modules

- [Serial](https://www.drupal.org/project/serial)
- [Computed Fields](https://www.drupal.org/project/computed_field)
