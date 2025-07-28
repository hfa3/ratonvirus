# v0.4.4

Support for Rails 8

Changed:

- The minimum Ruby version is now set to 3.2 as it is a requirement of Rails 8

# v0.4.3

Fixed:

- Manual scan is not working for File objects #32

# v0.4.2

Fixed:

- Issue with ActiveStorage file integrity check due to IO position change after the virus check

# v0.4.1

Fixed:

- Issue related to the EICAR test scanner. Related to [#16](https://github.com/mainio/ratonvirus/pull/16)

# v0.4.0

Support for Rails 7

Changed:

- The minimum Ruby version is now set to 2.7 as it is a requirement of Rails 7

# v0.3.2

Fixed:

- Backport: Issue with ActiveStorage file integrity check due to IO position change after the virus check

# v0.3.1

Fixed:

- Backport: Issue related to the EICAR test scanner. Related to [#16](https://github.com/mainio/ratonvirus/pull/16)

# v0.3.0

Changed:

- Minimum Ruby version is now set to 2.5

Fixed:

- Issue related with scanning files with CarrierWave storage engine using remote storage engines such as Fog. Related
  to [#9](https://github.com/mainio/ratonvirus/pull/9)

# v0.2.0

Support for Rails 6

The ActiveStorage storage engine has been updated and partly rewritten due to changes in its API. The new API introduces
a changes concept in the library which this update takes in to account. In the new API, the blobs will not get uploaded
to the storage service before the validations have been successful, which led to rethinking how this storage engine
works in Ratonvirus.

# v0.1.2

Fixed:

- Backport: Issue related with scanning files with CarrierWave storage engine using remote storage engines such as Fog.
  Related to #9

# v0.1.1

Fixed:

- Rescue file not found exception for blob.download [#2](https://github.com/mainio/ratonvirus/pull/2)

# v0.1.0

Initial public release.
