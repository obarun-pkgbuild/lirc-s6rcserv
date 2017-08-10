# Maintainer: Eric Vidal <eric@obarun.org>

pkgname=lirc-s6rcserv
pkgver=0.1
pkgrel=2
pkgdesc="lirc service for s6"
arch=(x86_64)
license=('beerware')
depends=('lirc' 's6' 's6-rc' 's6-boot')
conflicts=()
install=lirc-s6rcserv.install
source=('lirc.prepare-daemon.dependencies.s6'
		'lirc.prepare-daemon.type.s6'
		'lirc.prepare-daemon.up.s6'

		'lircd.daemon.dependencies.s6'
		'lircd.daemon.pipeline-name.s6'
		'lircd.daemon.producer-for.s6'
		'lircd.daemon.run.s6'
		'lircd.daemon.type.s6'

		'lircd.log.consumer-for.s6'
		'lircd.log.dependencies.s6'
		'lircd.log.run.s6'
		'lircd.log.type.s6'
		
		'lircmd.daemon.dependencies.s6'
		'lircmd.daemon.pipeline-name.s6'
		'lircmd.daemon.producer-for.s6'
		'lircmd.daemon.run.s6'
		'lircmd.daemon.type.s6'

		'lircmd.log.consumer-for.s6'
		'lircmd.log.dependencies.s6'
		'lircmd.log.run.s6'
		'lircmd.log.type.s6'
		
		'bundle.lirc.contents.s6'
		'bundle.lirc.type.s6'
		'LICENSE')
md5sums=('68b329da9893e34099c7d8ad5cb9c940'
         '85bceea1fb94d4166f24496dc40a35e6'
         'd93680e1dfb1d17865097918a9437bda'
         '3907cdef6349321b8d2e81d742c0f124'
         'd4838cf9c993e3081c799c621fe0b272'
         '89c4278b016cb42a3a535f2bb686ad94'
         'bb62b43e7c84672e6a1afb2891c57056'
         '42c13bdd7f61c06ac59c1aaca9c0f07a'
         'b5fb7cea445c7c9b1228d6ed31fd21b0'
         '68b329da9893e34099c7d8ad5cb9c940'
         '83cf918efdbaf3e0e80a95159808864c'
         '42c13bdd7f61c06ac59c1aaca9c0f07a'
         '3907cdef6349321b8d2e81d742c0f124'
         'fcdeff9622f7449d27c4cd0536e364cd'
         '4a57c94991843cdfc2f8c889a2b3a874'
         'bb1d8eef17f5dee0b5273ef5658071cb'
         '42c13bdd7f61c06ac59c1aaca9c0f07a'
         'b73972f43cb53fbb35af629f2a364579'
         '68b329da9893e34099c7d8ad5cb9c940'
         '9dd8859940add642e188ffe5eeb2c7ef'
         '42c13bdd7f61c06ac59c1aaca9c0f07a'
         '895652a7c208f9bcf13cf3086cdd5fa9'
         '71abe97e2554d37f1d12c5bf4945297f'
         '191a37ae657aa17e37e75d0242865dba')

package() {
	
	# bundle , trouble here user-lirc need a maj at lirc e.g user-Base
	install -Dm 0644 "$srcdir/bundle.lirc.contents.s6" "$pkgdir/etc/s6-serv/available/rc/bundle-Lirc/contents"
	install -Dm 0644 "$srcdir/bundle.lirc.type.s6" "$pkgdir/etc/s6-serv/available/rc/bundle-Lirc/type"
	
	# prepare
	install -Dm 0644 "$srcdir/lirc.prepare-daemon.dependencies.s6" "$pkgdir/etc/s6-serv/available/rc/lirc-prepare/dependencies"
	install -Dm 0644 "$srcdir/lirc.prepare-daemon.type.s6" "$pkgdir/etc/s6-serv/available/rc/lirc-prepare/type"
	install -Dm 0644 "$srcdir/lirc.prepare-daemon.up.s6" "$pkgdir/etc/s6-serv/available/rc/lirc-prepare/up"
	
	# daemon lircd
	install -Dm 0644 "$srcdir/lircd.daemon.dependencies.s6" "$pkgdir/etc/s6-serv/available/rc/lircd-daemon/dependencies"
	install -Dm 0644 "$srcdir/lircd.daemon.pipeline-name.s6" "$pkgdir/etc/s6-serv/available/rc/lircd-daemon/pipeline-name"
	install -Dm 0644 "$srcdir/lircd.daemon.producer-for.s6" "$pkgdir/etc/s6-serv/available/rc/lircd-daemon/producer-for"
	install -Dm 0644 "$srcdir/lircd.daemon.run.s6" "$pkgdir/etc/s6-serv/available/rc/lircd-daemon/run"
	install -Dm 0644 "$srcdir/lircd.daemon.type.s6" "$pkgdir/etc/s6-serv/available/rc/lircd-daemon/type"
	
	# log
	install -Dm 0644 "$srcdir/lircd.log.consumer-for.s6" "$pkgdir/etc/s6-serv/available/rc/lircd-log/consumer-for"
	install -Dm 0644 "$srcdir/lircd.log.dependencies.s6" "$pkgdir/etc/s6-serv/available/rc/lircd-log/dependencies"
	install -Dm 0644 "$srcdir/lircd.log.run.s6" "$pkgdir/etc/s6-serv/available/rc/lircd-log/run"
	install -Dm 0644 "$srcdir/lircd.log.type.s6" "$pkgdir/etc/s6-serv/available/rc/lircd-log/type"
	
	# daemon lircmd
	install -Dm 0644 "$srcdir/lircmd.daemon.dependencies.s6" "$pkgdir/etc/s6-serv/available/rc/lircmd-daemon/dependencies"
	install -Dm 0644 "$srcdir/lircmd.daemon.pipeline-name.s6" "$pkgdir/etc/s6-serv/available/rc/lircmd-daemon/pipeline-name"
	install -Dm 0644 "$srcdir/lircmd.daemon.producer-for.s6" "$pkgdir/etc/s6-serv/available/rc/lircmd-daemon/producer-for"
	install -Dm 0644 "$srcdir/lircmd.daemon.run.s6" "$pkgdir/etc/s6-serv/available/rc/lircmd-daemon/run"
	install -Dm 0644 "$srcdir/lircmd.daemon.type.s6" "$pkgdir/etc/s6-serv/available/rc/lircmd-daemon/type"
	
	# log
	install -Dm 0644 "$srcdir/lircmd.log.consumer-for.s6" "$pkgdir/etc/s6-serv/available/rc/lircmd-log/consumer-for"
	install -Dm 0644 "$srcdir/lircmd.log.dependencies.s6" "$pkgdir/etc/s6-serv/available/rc/lircmd-log/dependencies"
	install -Dm 0644 "$srcdir/lircmd.log.run.s6" "$pkgdir/etc/s6-serv/available/rc/lircmd-log/run"
	install -Dm 0644 "$srcdir/lircmd.log.type.s6" "$pkgdir/etc/s6-serv/available/rc/lircmd-log/type"
	
	install -Dm 0644 "$srcdir/LICENSE" "$pkgdir/usr/share/licenses/lirc-s6rcserv/LICENSE"
}
