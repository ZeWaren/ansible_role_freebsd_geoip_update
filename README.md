# ansible-freebsd-geoip-update

## Introduction
This role installs and configure `geoipupdate` on FreeBSD.

## Variables

See [defaults/main.yml](defaults/main.yml) for the default values of each.

### geoip_update_edition_ids

Which editions of the databases to download.

### geoip_update_account_id

Your maxmind account ID.

### geoip_update_license_key

Your maxmind licence key.

## Example

### Download the free edition of the country database

	geoip_update_edition_ids: GeoLite2-Country

### Download the paid edition of the country and city databases

	geoip_update_edition_ids: GeoLite2-Country GeoLite2-City
	geoip_update_account_id: "123456789"
	geoip_update_license_key: "10111213141516"

## Dependencies

None.

## Licence

BSD

## Author

[Erwan Martin](https://zewaren.net/)
