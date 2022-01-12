Changelog
=========

0.7.2 (2022-01-12)
------------------
- Fix incorrect initialization through hook

0.7.1 (2021-11-03)
------------------
- Initialize memory with empty dict avoiding logs
- Call serialization with buffer instead of memoryview
- Treat null bytes on JSON loads

0.7.0 (2021-10-26)
------------------
- Run CI on different python versions
- Add support for python 3.10
- Improve README with more examples and calls to close and unlink
- Expose shared memory as readonly attribute as ShareableList
- Modify SharedMemoryDict to use serializers
- Create serializers for json and pickle

0.6.0 (2021-10-20)
------------------
- Replace SENTINEL with NOT_GIVEN
- Update project dependencies
- Add a better message on the storage issue

0.5.0 (2021-02-11)
------------------
- Configure black as formatter
- Implement Mapping interface (all methods)
- Deprecate `move_to_end and` method and `last` parameter on `popitem`

0.4.0 (2020-11-09)
------------------
- Remove method `validate_key` from Django adapter (this is a method to deal with memcached key name issues)
- Decrease shared-memory and pickle calls on Django Adapter
- Raise `TypeError` on `incr` method of Django Adapter for non int values
- Remover `cull` mechanism from django adapter

0.3.1 (2020-10-26)
------------------
- Prevent `KeyError` and `IndexError` on checking expire of Django cache adapter

0.3.0 (2020-10-21)
------------------
- Remove uwsgi lock and use `multiprocessing.Lock` instead

0.2.0 (2020-10-19)
------------------
- Using lock on method `SharedMemoryDict.clear()`

0.1.1 (2020-08-12)
------------------
- Fix typo on hooks
- Remove name-prefix of caches (django and aiocache)

0.1.0 (2020-08-05)
------------------
- First Release :tada:
