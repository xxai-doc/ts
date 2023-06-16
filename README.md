<p align="center"><a href="https://xxai.art"><img src="https://cdn.jsdelivr.net/gh/xxai-art/doc/logo.svg"/></a><br/><a href="https://xxai.art"><img src="https://cdn.jsdelivr.net/gh/xxai-art/doc/xxai.svg"/></a></p><p align="center"><a href="https://github.com/xxai-art/doc#readme"><img alt="I18N" src="https://cdn.jsdelivr.net/gh/wactax/img/t.svg"/></a>　<a href="https://groups.google.com/u/0/g/xxai-art"><img alt="Google Groups" src="https://cdn.jsdelivr.net/gh/wactax/img/g-groups.svg"/></a></p>

Swi ringanyetiwa ku nghenisa nodejs, [direnv](https://direnv.net) , [bun](https://github.com/oven-sh/bun) ku sungula, ivi `direnv allow` endzhaku ko nghena eka xikombo ( [.envrc](https://github.com/xxai-art/doc/blob/main/.envrc) yi ta tirhisiwa hi ku tisungulela endzhaku ko nghena eka xikombo).

Nhlamuselo ya kona hi leyi: Vuhundzuluxeri bya Xichayina eka Xijapani, Xikorea, Xinghezi, Vuhundzuluxeri bya Xinghezi eka tindzimi tin’wana hinkwato. Loko u lava ku seketela Xichayina na Xinghezi ntsena, u nga tsala ntsena `zh: en` .

## khodi ya le mahlweni

* [khodi ya le mahlweni](https://github.com/xxai-art/web)
* [Tiphakiti ta ririmi ta sayiti hi ku angarhela](https://github.com/xxai-art/web/tree/main/i18n)
* [Tiphakiti ta ririmi ta mimojula yo nghena](https://github.com/wacpkg/user/tree/main/ui.i18n)
* [Website Matsalwa ya Tindzimi to Tala](https://github.com/xxai-doc)

Ririmi ra minongonoko ya le mahlweni i [@w5/coffee_plus](http://npmjs.com/@w5/coffee_plus) , leri engetelaka swihlawulekisi swin’wana leswi simekiweke eka xivumbeko xa coffeescript, vona [./coffee_plus.md](./coffee_plus.md) .

## Ku endliwa ka tiwebsite na matsalwa ya matiko ya misava

Aka eka tiphurojeke ta 3 leti landzelaka

* [@w5/mdt](https://www.npmjs.com/package/@w5/mdt)

  Xilandzi i `.mdt` , u nga tirhisa xivumbeko xa marito lexi fanaka na `<+ ./coffee_plus/import.js>` ku kongomisa eka tifayela ta le handle, naswona u tumbuluxa markdown hi xilandzi `.md` .

* [@w5/trmd hi ku tirhisa](https://www.npmjs.com/package/@w5/trmd)

  Vuhundzuluxi bya Markdown a byi nge hundzuluxeli tikhodi na swihlanganisi, naswona byi ta hlayisa swivulwa leswi hundzuluxeriweke. Loko vuhundzuluxeri byi cinciwile kambe tsalwa ro sungula ri nga cinciwanga, ku byi hetisisa nakambe a swi nge tsali ehenhla ka ku cinciwa ka vuhundzuluxeri.

* [@w5/i18n](https://www.npmjs.com/package/@w5/i18n)

  Tifayili ta ririmi to hundzuluxela tiwebsite leti endliweke hi `yaml` .

### Swiletelo swa Vuhundzuluxi bya Matsalwa ya Xiothomethi

Vona vuhlayiselo bya khodi [xxai-art/doc](https://github.com/xxai-art/doc)

Swi ringanyetiwa ku nghenisa nodejs, [direnv](https://direnv.net) , [bun](https://github.com/oven-sh/bun) ku sungula, ivi `direnv allow` endzhaku ko nghena eka xikombo ( [.envrc](https://github.com/xxai-art/doc/blob/main/.envrc) yi ta tirhisiwa hi ku tisungulela endzhaku ko nghena eka xikombo).

Leswaku ndzi papalata xisekelo lexikulu xa khodi lexi hundzuluxeriweke eka madzana ya tindzimi, ndzi endle xisekelo xa khodi lexi hambaneke xa ririmi rin’wana ni rin’wana naswona ndzi endle nhlangano wo hlayisa xisekelo xa khodi

Ku veka xihlawulekisi xa ndhawu `GITHUB_ACCESS_TOKEN` ivi u tirhisa [create.github.coffee](https://github.com/xxai-art/doc/blob/main/create.github.coffee) swi ta tumbuluxa hi ku tisungulela vuhlayiselo bya khodi.

I ntiyiso leswaku u nga ha tlhela u yi veka eka xisekelo xa khodi.

Xikombo xa tsalwa ra vuhundzuluxi [run.sh](https://github.com/xxai-art/doc/blob/main/run.sh)

Khodi ya tsalwa yi hlamuseriwa hi ndlela leyi landzelaka:

[bunx](https://bun.sh/docs/cli/bunx) i xisirhelelo xa npx, lexi hatlisaka. I ntiyiso, loko u nga ri na bun leyi nghenisiweke, u nga tirhisa `npx` ematshan’wini ya sweswo.

`bunx mdt zh` yi hundzuluxela `.mdt` eka xikombo xa zh tanihi `.md` , vona tifayela ta 2 leti hlanganisiweke laha hansi

* [kofi_ku engetela.mdt](https://github.com/xxai-doc/zh/blob/main/coffee_plus.mdt)
* [kofi_ku engetela.md](https://github.com/xxai-doc/zh/blob/main/coffee_plus.md)

`bunx i18n` i khodi ya nkoka ya vuhundzuluxi (loko u ri na `nodejs` leti nghenisiweke ntsena, kambe `bun` na `direnv` ti nga nghenisiwanga, u nga ha tlhela u tirhisa `npx i18n` ku ​​hundzuluxela).

Yi ta parse [i18n.yml](https://github.com/xxai-art/doc/blob/main/i18n.yml) , vukorhokeri bya `i18n.yml` eka tsalwa leri byi le ka xiyimo lexi landzelaka:

```
en:
zh: ja ko en
```

Nhlamuselo ya kona hi leyi: Vuhundzuluxeri bya Xichayina eka Xijapani, Xikorea, Xinghezi, Vuhundzuluxeri bya Xinghezi eka tindzimi tin’wana hinkwato. Loko u lava ku seketela Xichayina na Xinghezi ntsena, u nga tsala ntsena `zh: en` .

Xo hetelela i [gen.README.coffee](https://github.com/xxai-art/doc/blob/main/gen.README.coffee) , leyi humesaka leswi nga endzeni exikarhi ka nhlokomhaka leyikulu na nhlokomhaka-ntsongo yo sungula ya `README.md` ya ririmi rin’wana na rin’wana ku tumbuluxa ku nghena ka `README.md` . Khodi ya kona yi olovile swinene, u nga yi languta hi wexe.

Google API yi tirhisiwa eka vuhundzuluxeri bya mahala. Loko u nga swi koti ku nghena eka Google, hi kombela u lulamisa no veka proxy, ku fana na:

```
export https_proxy=http://127.0.0.1:7890 http_proxy=http://127.0.0.1:7890 all_proxy=socks5://127.0.0.1:7890
```

Tsalwa ra vuhundzuluxi ri ta tumbuluxa cache leyi hundzuluxeriweke eka `.i18n` directory, hi kombela u yi kambela hi `git status` naswona u yi engetela eka vuhlayiselo bya khodi ku papalata vuhundzuluxi lebyi phindha-phindhiweke.

Hi kombela u tirhisa `bunx i18n` nkarhi wun’wana na wun’wana loko u cinca vuhundzuluxeri ku pfuxeta cache.

Loko tsalwa ro sungula na vuhundzuluxeri swi cinciwile hi nkarhi wun’we, cache yi ta pfilunganyeka, kutani loko u lava ku cinca, u nga cinca yin’we ntsena, ivi u tirhisa `bunx i18n` ku ​​pfuxeta cache.
