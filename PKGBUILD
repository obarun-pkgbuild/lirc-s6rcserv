# Maintainer: Eric Vidal <eric@obarun.org>

pkgname=lirc-s6rcserv
pkgver=0.1
pkgrel=3
pkgdesc="lirc service for"
arch=(x86_64)
license=('beerware')
depends=('lirc' 's6' 's6-rc' 's6-boot')
conflicts=()
source=('lirc.prepare.dependencies'
		'lirc.prepare.type'
		'lirc.prepare.up'

		'lircd.longrun.dependencies'
		'lircd.longrun.pipeline-name'
		'lircd.longrun.producer-for'
		'lircd.longrun.run'
		'lircd.longrun.type'

		'lircd.log.consumer-for'
		'lircd.log.dependencies'
		'lircd.log.run'
		'lircd.log.type'
		
		'lircmd.longrun.dependencies'
		'lircmd.longrun.pipeline-name'
		'lircmd.longrun.producer-for'
		'lircmd.longrun.run'
		'lircmd.longrun.type'

		'lircmd.log.consumer-for'
		'lircmd.log.dependencies'
		'lircmd.log.run'
		'lircmd.log.type'
		
		'bundle.lirc.contents'
		'bundle.lirc.type'
		'lirc.logd'
		'LICENSE')
md5sums=('68b329da9893e34099c7d8ad5cb9c940'
         '85bceea1fb94d4166f24496dc40a35e6'
         'd93680e1dfb1d17865097918a9437bda'
         '3907cdef6349321b8d2e81d742c0f124'
         'd4838cf9c993e3081c799c621fe0b272'
         '89c4278b016cb42a3a535f2bb686ad94'
         'bb62b43e7c84672e6a1afb2891c57056'
         '42c13bdd7f61c06ac59c1aaca9c0f07a'
         '9ed6841d9184d79a2fae778396268577'
         '68b329da9893e34099c7d8ad5cb9c940'
         '83cf918efdbaf3e0e80a95159808864c'
         '42c13bdd7f61c06ac59c1aaca9c0f07a'
         '3907cdef6349321b8d2e81d742c0f124'
         'fcdeff9622f7449d27c4cd0536e364cd'
         '4a57c94991843cdfc2f8c889a2b3a874'
         'bb1d8eef17f5dee0b5273ef5658071cb'
         '42c13bdd7f61c06ac59c1aaca9c0f07a'
         '08375643659768b630b76d8946ce8f32'
         '68b329da9893e34099c7d8ad5cb9c940'
         '9dd8859940add642e188ffe5eeb2c7ef'
         '42c13bdd7f61c06ac59c1aaca9c0f07a'
         '9de6b4d62b7651ea5e2db4c9d6744076'
         '71abe97e2554d37f1d12c5bf4945297f'
         '201511bb215d4fe78d9a1e76fe8166fd'
         '191a37ae657aa17e37e75d0242865dba')

package() {
	
	# bundle , trouble here user-lirc need a maj at lirc e.g user-Base
	install -Dm 0644 "$srcdir/bundle.lirc.contents" "$pkgdir/etc/s6-serv/available/rc/bundle-Lirc/contents"
	install -Dm 0644 "$srcdir/bundle.lirc.type" "$pkgdir/etc/s6-serv/available/rc/bundle-Lirc/type"
	
	# prepare
	install -Dm 0644 "$srcdir/lirc.prepare.dependencies" "$pkgdir/etc/s6-serv/available/rc/lirc-prepare/dependencies"
	install -Dm 0644 "$srcdir/lirc.prepare.type" "$pkgdir/etc/s6-serv/available/rc/lirc-prepare/type"
	install -Dm 0644 "$srcdir/lirc.prepare.up" "$pkgdir/etc/s6-serv/available/rc/lirc-prepare/up"
	
	# longrun lircd
	install -Dm 0644 "$srcdir/lircd.longrun.dependencies" "$pkgdir/etc/s6-serv/available/rc/lircd-longrun/dependencies"
	install -Dm 0644 "$srcdir/lircd.longrun.pipeline-name" "$pkgdir/etc/s6-serv/available/rc/lircd-longrun/pipeline-name"
	install -Dm 0644 "$srcdir/lircd.longrun.producer-for" "$pkgdir/etc/s6-serv/available/rc/lircd-longrun/producer-for"
	install -Dm 0644 "$srcdir/lircd.longrun.run" "$pkgdir/etc/s6-serv/available/rc/lircd-longrun/run"
	install -Dm 0644 "$srcdir/lircd.longrun.type" "$pkgdir/etc/s6-serv/available/rc/lircd-longrun/type"
	
	# log
	install -Dm 0644 "$srcdir/lircd.log.consumer-for" "$pkgdir/etc/s6-serv/available/rc/lircd-log/consumer-for"
	install -Dm 0644 "$srcdir/lircd.log.dependencies" "$pkgdir/etc/s6-serv/available/rc/lircd-log/dependencies"
	install -Dm 0644 "$srcdir/lircd.log.run" "$pkgdir/etc/s6-serv/available/rc/lircd-log/run"
	install -Dm 0644 "$srcdir/lircd.log.type" "$pkgdir/etc/s6-serv/available/rc/lircd-log/type"
	
	# longrun lircmd
	install -Dm 0644 "$srcdir/lircmd.longrun.dependencies" "$pkgdir/etc/s6-serv/available/rc/lircmd-longrun/dependencies"
	install -Dm 0644 "$srcdir/lircmd.longrun.pipeline-name" "$pkgdir/etc/s6-serv/available/rc/lircmd-longrun/pipeline-name"
	install -Dm 0644 "$srcdir/lircmd.longrun.producer-for" "$pkgdir/etc/s6-serv/available/rc/lircmd-longrun/producer-for"
	install -Dm 0644 "$srcdir/lircmd.longrun.run" "$pkgdir/etc/s6-serv/available/rc/lircmd-longrun/run"
	install -Dm 0644 "$srcdir/lircmd.longrun.type" "$pkgdir/etc/s6-serv/available/rc/lircmd-longrun/type"
	
	# log
	install -Dm 0644 "$srcdir/lircmd.log.consumer-for" "$pkgdir/etc/s6-serv/available/rc/lircmd-log/consumer-for"
	install -Dm 0644 "$srcdir/lircmd.log.dependencies" "$pkgdir/etc/s6-serv/available/rc/lircmd-log/dependencies"
	install -Dm 0644 "$srcdir/lircmd.log.run" "$pkgdir/etc/s6-serv/available/rc/lircmd-log/run"
	install -Dm 0644 "$srcdir/lircmd.log.type" "$pkgdir/etc/s6-serv/available/rc/lircmd-log/type"
	
	# hook
	install -Dm 0644 "$srcdir/lirc.logd" "$pkgdir/etc/s6-serv/log.d/lirc-rc"
	
	install -Dm 0644 "$srcdir/LICENSE" "$pkgdir/usr/share/licenses/lirc-s6rcserv/LICENSE"
}
