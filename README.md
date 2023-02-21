def menu():
	try:sh = requests.get('https://httpbin.org/ip').json()
	except:sh = {'origin':'-'}
	try:
		tglx = my_birthday.split('/')[1]
		blnx = dic2[str(my_birthday.split('/')[0])]
		thnx = my_birthday.split('/')[2]
		birth = tglx+' '+blnx+' '+thnx
	except:birth = '-'
	banner()
	sg = '# INFORMASI USER'
	fx = mark(sg, style='red')
	sol().print(fx)
	#print(x+'['+h+'•'+x+'] \033[0;34mNama Akun Sia  : '+str(my_name))
	#print(x+'['+h+'•'+x+'] \033[0;34mID Akun Sua    : '+str(my_id))
	#print(x+'['+h+'•'+x+'] \033[93mTanggal Croot  : '+str(birth))
	print(x+'['+h+'•'+x+'] \033[923mAlamat Ip    : '+str(sh['origin']))
	io = '\x1b[1;92m[01] Crack Dari Pertemanan Publik\n\x1b[1;92m[02] Crack ID Dari Akun Publik (masal) \n\x1b[1;92m[03] Crack Dari Grup\n\x1b[1;92m[04] Bot Share Fb\n\x1b[1;92m[05] Crack Follower Fb\n\x1b[1;92m[06] Cek Hasil Crack\n\x1b[1;92m[07] Gantin User Agent\n\033\x1b[1;92m[08] Cek Hasil Crack\n[00] Keluar'
	oi = nel(io, style='cyan')
	cetak(nel(oi, title='PILIHAN MENU'))
	jh = input(x+'['+p+'•'+x+'] Pilih : ')
	if jh in ['1','01']:
		dump_publik()
	elif jh in ['2','02']:		
		dump_massal()
	elif jh in ['3','03']:
		grup()
	elif jh in ['4','04']:
		 main()
	elif jh in ['5','05']:
		follower()
	elif jh in ['6','06']:
		result()
	elif jh in ['7','07']:
		useragent()
	elif jh in ['8','08']:
		file()
	elif jh in ['0','00']:
		os.system('rm -rf .token.txt')
		print(x+'['+h+'•'+x+'] Tunggu ...')
		time.sleep(1)
		sw = '# SUKSES KELUAR'
		sol().print(mark(sw, style='green'
