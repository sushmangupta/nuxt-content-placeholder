# Update Shopware

Your Shopware updates are essential for maintaining security, fixing bugs, and improving performance. They protect against new cyber threats by patching vulnerabilities, enhance the software's stability, and often introduce new features or optimizations. Regular updates also ensure compatibility with the latest technologies and compliance with legal requirements, helping to keep the software functional, secure, and up-to-date.
There are different types of releases that can contain different types of changes. The release process also varies depending on the distribution type of Shopware. For the SaaS version of Shopware a continuous delivery process is in place where forward-compatible changes are deployed once a week. For the self-hosted version of Shopware a typical semantic versioning system is in place which includes the following releases.

## What are the types of releases and frequency ?

| Release type | Details | Frequency |
|--------------|---------|-----------|
| Major | Its a biggest form of a release. It focuses primarily on technical improvements and its the only type of release that allows for breaking changes. In this all the deprecated code parts of previous major cycle are removed, 3rd party frameworks are updated, minimum system requirements are raised and those features flagged as `@experimental` are moved to stable. | Once  a year |
| Minor | Its the most common release type and is used to deliver recent bug fixes and new forward-compatible features to our customers. | Every first Monday of the month |
| Patch | Its performed on demand and their scope is limited to the necessary fix - critical issues or security vulnerabilities | On demand |

To perform these updates follow the [guidelines](https://docs.shopware.com/en/shopware-6-en/update-guides/updating-shopware)

## What is the most recommended way?

The most recommended way is composer update.

However, before you perform a successful update, its necesaary to a backup of your existing data. Take a look about it in the next section.
