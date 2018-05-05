# 获取中国大陆休假日

## 测试

```python
print(getYearHolidays("2019"))
print(getYearHolidays())
print(getYearHolidays("2017"))
print(getYearHolidays("2016"))
print(getYearHolidays("2015"))
print(getMonthHolidays("201708"))
print(getDayHoliday("20170501"))
```

## 结果

```log
只等查 2018、2017 和 2016 年的节假日
None
爬取地址: http://holidays-calendar.net/calendar_zh_cn/china_zh_cn.html
{'201801': {'20180101': 2, '20180102': 0, '20180103': 0, '20180104': 0, '20180105': 0, '20180106': 1, '20180107': 1, '20180108': 0, '20180109': 0, '20180110': 0, '20180111': 0, '20180112': 0, '20180113': 1, '20180114': 1, '20180115': 0, '20180116': 0, '20180117': 0, '20180118': 0, '20180119': 0, '20180120': 1, '20180121': 1, '20180122': 0, '20180123': 0, '20180124': 0, '20180125': 0, '20180126': 0, '20180127': 1, '20180128': 1, '20180129': 0, '20180130': 0, '20180131': 0}, '201802': {'20180201': 0, '20180202': 0, '20180203': 1, '20180204': 1, '20180205': 0, '20180206': 0, '20180207': 0, '20180208': 0, '20180209': 0, '20180210': 1, '20180211': 0, '20180212': 0, '20180213': 0, '20180214': 0, '20180215': 2, '20180216': 2, '20180217': 2, '20180218': 2, '20180219': 2, '20180220': 2, '20180221': 2, '20180222': 0, '20180223': 0, '20180224': 0, '20180225': 1, '20180226': 0, '20180227': 0, '20180228': 0}, '201803': {'20180301': 0, '20180302': 0, '20180303': 1, '20180304': 1, '20180305': 0, '20180306': 0, '20180307': 0, '20180308': 0, '20180309': 0, '20180310': 1, '20180311': 1, '20180312': 0, '20180313': 0, '20180314': 0, '20180315': 0, '20180316': 0, '20180317': 1, '20180318': 1, '20180319': 0, '20180320': 0, '20180321': 0, '20180322': 0, '20180323': 0, '20180324': 1, '20180325': 1, '20180326': 0, '20180327': 0, '20180328': 0, '20180329': 0, '20180330': 0, '20180331': 1}, '201804': {'20180401': 1, '20180402': 0, '20180403': 0, '20180404': 0, '20180405': 2, '20180406': 2, '20180407': 2, '20180408': 0, '20180409': 0, '20180410': 0, '20180411': 0, '20180412': 0, '20180413': 0, '20180414': 1, '20180415': 1, '20180416': 0, '20180417': 0, '20180418': 0, '20180419': 0, '20180420': 0, '20180421': 1, '20180422': 1, '20180423': 0, '20180424': 0, '20180425': 0, '20180426': 0, '20180427': 0, '20180428': 0, '20180429': 2, '20180430': 2}, '201805': {'20180501': 2, '20180502': 0, '20180503': 0, '20180504': 0, '20180505': 1, '20180506': 1, '20180507': 0, '20180508': 0, '20180509': 0, '20180510': 0, '20180511': 0, '20180512': 1, '20180513': 1, '20180514': 0, '20180515': 0, '20180516': 0, '20180517': 0, '20180518': 0, '20180519': 1, '20180520': 1, '20180521': 0, '20180522': 0, '20180523': 0, '20180524': 0, '20180525': 0, '20180526': 1, '20180527': 1, '20180528': 0, '20180529': 0, '20180530': 0, '20180531': 0}, '201806': {'20180601': 0, '20180602': 1, '20180603': 1, '20180604': 0, '20180605': 0, '20180606': 0, '20180607': 0, '20180608': 0, '20180609': 1, '20180610': 1, '20180611': 0, '20180612': 0, '20180613': 0, '20180614': 0, '20180615': 0, '20180616': 2, '20180617': 2, '20180618': 2, '20180619': 0, '20180620': 0, '20180621': 0, '20180622': 0, '20180623': 1, '20180624': 1, '20180625': 0, '20180626': 0, '20180627': 0, '20180628': 0, '20180629': 0, '20180630': 1}, '201808': {'20180801': 0, '20180802': 0, '20180803': 0, '20180804': 1, '20180805': 1, '20180806': 0, '20180807': 0, '20180808': 0, '20180809': 0, '20180810': 0, '20180811': 1, '20180812': 1, '20180813': 0, '20180814': 0, '20180815': 0, '20180816': 0, '20180817': 0, '20180818': 1, '20180819': 1, '20180820': 0, '20180821': 0, '20180822': 0, '20180823': 0, '20180824': 0, '20180825': 1, '20180826': 1, '20180827': 0, '20180828': 0, '20180829': 0, '20180830': 0, '20180831': 0}, '201810': {'20181001': 2, '20181002': 2, '20181003': 2, '20181004': 2, '20181005': 2, '20181006': 2, '20181007': 2, '20181008': 0, '20181009': 0, '20181010': 0, '20181011': 0, '20181012': 0, '20181013': 1, '20181014': 1, '20181015': 0, '20181016': 0, '20181017': 0, '20181018': 0, '20181019': 0, '20181020': 1, '20181021': 1, '20181022': 0, '20181023': 0, '20181024': 0, '20181025': 0, '20181026': 0, '20181027': 1, '20181028': 1, '20181029': 0, '20181030': 0, '20181031': 0}, '201811': {'20181101': 0, '20181102': 0, '20181103': 1, '20181104': 1, '20181105': 0, '20181106': 0, '20181107': 0, '20181108': 0, '20181109': 0, '20181110': 1, '20181111': 1, '20181112': 0, '20181113': 0, '20181114': 0, '20181115': 0, '20181116': 0, '20181117': 1, '20181118': 1, '20181119': 0, '20181120': 0, '20181121': 0, '20181122': 0, '20181123': 0, '20181124': 1, '20181125': 1, '20181126': 0, '20181127': 0, '20181128': 0, '20181129': 0, '20181130': 0}, '201812': {'20181201': 1, '20181202': 1, '20181203': 0, '20181204': 0, '20181205': 0, '20181206': 0, '20181207': 0, '20181208': 1, '20181209': 1, '20181210': 0, '20181211': 0, '20181212': 0, '20181213': 0, '20181214': 0, '20181215': 1, '20181216': 1, '20181217': 0, '20181218': 0, '20181219': 0, '20181220': 0, '20181221': 0, '20181222': 1, '20181223': 1, '20181224': 0, '20181225': 0, '20181226': 0, '20181227': 0, '20181228': 0, '20181229': 1, '20181230': 1, '20181231': 0}}
爬取地址: http://holidays-calendar.net/2017/calendar_zh_cn/china_zh_cn.html
{'201701': {'20170101': 2, '20170102': 2, '20170103': 0, '20170104': 0, '20170105': 0, '20170106': 0, '20170107': 1, '20170108': 1, '20170109': 0, '20170110': 0, '20170111': 0, '20170112': 0, '20170113': 0, '20170114': 1, '20170115': 1, '20170116': 0, '20170117': 0, '20170118': 0, '20170119': 0, '20170120': 0, '20170121': 1, '20170122': 0, '20170123': 0, '20170124': 0, '20170125': 0, '20170126': 0, '20170127': 2, '20170128': 2, '20170129': 2, '20170130': 2, '20170131': 2}, '201702': {'20170201': 2, '20170202': 2, '20170203': 0, '20170204': 0, '20170205': 1, '20170206': 0, '20170207': 0, '20170208': 0, '20170209': 0, '20170210': 0, '20170211': 1, '20170212': 1, '20170213': 0, '20170214': 0, '20170215': 0, '20170216': 0, '20170217': 0, '20170218': 1, '20170219': 1, '20170220': 0, '20170221': 0, '20170222': 0, '20170223': 0, '20170224': 0, '20170225': 1, '20170226': 1, '20170227': 0, '20170228': 0}, '201703': {'20170301': 0, '20170302': 0, '20170303': 0, '20170304': 1, '20170305': 1, '20170306': 0, '20170307': 0, '20170308': 0, '20170309': 0, '20170310': 0, '20170311': 1, '20170312': 1, '20170313': 0, '20170314': 0, '20170315': 0, '20170316': 0, '20170317': 0, '20170318': 1, '20170319': 1, '20170320': 0, '20170321': 0, '20170322': 0, '20170323': 0, '20170324': 0, '20170325': 1, '20170326': 1, '20170327': 0, '20170328': 0, '20170339': 0, '20170330': 0, '20170331': 0}, '201704': {'20170401': 0, '20170402': 2, '20170403': 2, '20170404': 2, '20170405': 0, '20170406': 0, '20170407': 0, '20170408': 1, '20170409': 1, '20170410': 0, '20170411': 0, '20170412': 0, '20170413': 0, '20170414': 0, '20170415': 1, '20170416': 1, '20170417': 0, '20170418': 0, '20170419': 0, '20170420': 0, '20170421': 0, '20170422': 1, '20170423': 1, '20170424': 0, '20170425': 0, '20170426': 0, '20170427': 0, '20170428': 0, '20170429': 2, '20170430': 2}, '201705': {'20170501': 2, '20170502': 0, '20170503': 0, '20170504': 0, '20170505': 0, '20170506': 1, '20170507': 1, '20170508': 0, '20170509': 0, '20170510': 0, '20170511': 0, '20170512': 0, '20170513': 1, '20170514': 1, '20170515': 0, '20170516': 0, '20170517': 0, '20170518': 0, '20170519': 0, '20170520': 1, '20170521': 1, '20170522': 0, '20170523': 0, '20170524': 0, '20170525': 0, '20170526': 0, '20170527': 0, '20170528': 2, '20170529': 2, '20170530': 2, '20170531': 0}, '201706': {'20170601': 0, '20170602': 0, '20170603': 1, '20170604': 1, '20170605': 0, '20170606': 0, '20170607': 0, '20170608': 0, '20170609': 0, '20170610': 1, '20170611': 1, '20170612': 0, '20170613': 0, '20170614': 0, '20170615': 0, '20170616': 0, '20170617': 1, '20170618': 1, '20170619': 0, '20170620': 0, '20170621': 0, '20170622': 0, '20170623': 0, '20170624': 1, '20170625': 1, '20170626': 0, '20170627': 0, '20170628': 0, '20170629': 0, '20170630': 0}, '201708': {'20170801': 0, '20170802': 0, '20170803': 0, '20170804': 0, '20170805': 1, '20170806': 1, '20170807': 0, '20170808': 0, '20170809': 0, '20170810': 0, '20170811': 0, '20170812': 1, '20170813': 1, '20170814': 0, '20170815': 0, '20170816': 0, '20170817': 0, '20170818': 0, '20170819': 1, '20170820': 1, '20170821': 0, '20170822': 0, '20170823': 0, '20170824': 0, '20170825': 0, '20170826': 1, '20170827': 1, '20170828': 0, '20170829': 0, '20170830': 0, '20170831': 0}, '201710': {'20171001': 2, '20171002': 2, '20171003': 2, '20171004': 2, '20171005': 2, '20171006': 2, '20171007': 2, '20171008': 2, '20171009': 0, '20171010': 0, '20171011': 0, '20171012': 0, '20171013': 0, '20171014': 1, '20171015': 1, '20171016': 0, '20171017': 0, '20171018': 0, '20171019': 0, '20171020': 0, '20171021': 1, '20171022': 1, '20171023': 0, '20171024': 0, '20171025': 0, '20171026': 0, '20171027': 0, '20171028': 1, '20171029': 1, '20171030': 0, '20171031': 0}, '201711': {'20171101': 0, '20171102': 0, '20171103': 0, '20171104': 1, '20171105': 1, '20171106': 0, '20171107': 0, '20171108': 0, '20171109': 0, '20171110': 0, '20171111': 1, '20171112': 1, '20171113': 0, '20171114': 0, '20171115': 0, '20171116': 0, '20171117': 0, '20171118': 1, '20171119': 1, '20171120': 0, '20171121': 0, '20171122': 0, '20171123': 0, '20171124': 0, '20171125': 1, '20171126': 1, '20171127': 0, '20171128': 0, '20171129': 0, '20171130': 0}, '201712': {'20171201': 0, '20171202': 1, '20171203': 1, '20171204': 0, '20171205': 0, '20171206': 0, '20171207': 0, '20171208': 0, '20171209': 1, '20171210': 1, '20171211': 0, '20171212': 0, '20171213': 0, '20171214': 0, '20171215': 0, '20171216': 1, '20171217': 1, '20171218': 0, '20171219': 0, '20171220': 0, '20171221': 0, '20171222': 0, '20171223': 1, '20171224': 1, '20171225': 0, '20171226': 0, '20171227': 0, '20171228': 0, '20171229': 0, '20171230': 1, '20171231': 1}}
爬取地址: http://holidays-calendar.net/2016/calendar_zh_cn/china_zh_cn.html
{'201601': {'20160101': 2, '20160102': 2, '20160103': 2, '20160104': 0, '20160105': 0, '20160106': 0, '20160107': 0, '20160108': 0, '20160109': 1, '20160110': 1, '20160111': 0, '20160112': 0, '20160113': 0, '20160114': 0, '20160115': 0, '20160116': 1, '20160117': 1, '20160118': 0, '20160119': 0, '20160120': 0, '20160121': 0, '20160122': 0, '20160123': 1, '20160124': 1, '20160125': 0, '20160126': 0, '20160127': 0, '20160128': 0, '20160129': 0, '20160130': 1, '20160131': 1}, '201602': {'20160201': 0, '20160202': 0, '20160203': 0, '20160204': 0, '20160205': 0, '20160206': 0, '20160207': 2, '20160208': 2, '20160209': 2, '20160210': 2, '20160211': 2, '20160212': 2, '20160213': 2, '20160214': 0, '20160215': 0, '20160216': 0, '20160217': 0, '20160218': 0, '20160219': 0, '20160220': 1, '20160221': 1, '20160222': 0, '20160223': 0, '20160224': 0, '20160225': 0, '20160226': 0, '20160227': 1, '20160228': 1, '20160229': 0}, '201603': {'20160301': 0, '20160302': 0, '20160303': 0, '20160304': 0, '20160305': 1, '20160306': 1, '20160307': 0, '20160308': 0, '20160309': 0, '20160310': 0, '20160311': 0, '20160312': 1, '20160313': 1, '20160314': 0, '20160315': 0, '20160316': 0, '20160317': 0, '20160318': 0, '20160319': 1, '20160320': 1, '20160321': 0, '20160322': 0, '20160323': 0, '20160324': 0, '20160325': 0, '20160326': 1, '20160327': 1, '20160328': 0, '20160329': 0, '20160330': 0, '20160331': 0}, '201604': {'20160401': 0, '20160402': 2, '20160403': 2, '20160404': 2, '20160405': 0, '20160406': 0, '20160407': 0, '20160408': 0, '20160409': 1, '20160410': 1, '20160411': 0, '20160412': 0, '20160413': 0, '20160414': 0, '20160415': 0, '20160416': 1, '20160417': 1, '20160418': 0, '20160419': 0, '20160420': 0, '20160421': 0, '20160422': 0, '20160423': 1, '20160424': 1, '20160425': 0, '20160426': 0, '20160427': 0, '20160428': 0, '20160429': 0, '20160430': 2}, '201605': {'20160501': 2, '20160502': 2, '20160503': 0, '20160504': 0, '20160505': 0, '20160506': 0, '20160507': 1, '20160508': 1, '20160509': 0, '20160510': 0, '20160511': 0, '20160512': 0, '20160513': 0, '20160514': 1, '20160515': 1, '20160516': 0, '20160517': 0, '20160518': 0, '20160519': 0, '20160520': 0, '20160521': 1, '20160522': 1, '20160523': 0, '20160524': 0, '20160525': 0, '20160526': 0, '20160527': 0, '20160528': 1, '20160529': 1, '20160530': 0, '20160531': 0}, '201606': {'20160601': 0, '20160602': 0, '20160603': 0, '20160604': 1, '20160605': 1, '20160606': 0, '20160607': 0, '20160608': 0, '20160609': 2, '20160610': 2, '20160611': 2, '20160612': 0, '20160613': 0, '20160614': 0, '20160615': 0, '20160616': 0, '20160617': 0, '20160618': 1, '20160619': 1, '20160620': 0, '20160621': 0, '20160622': 0, '20160623': 0, '20160624': 0, '20160625': 1, '20160626': 1, '20160627': 0, '20160628': 0, '20160629': 0, '20160630': 0}, '201608': {'20160801': 0, '20160802': 0, '20160803': 0, '20160804': 0, '20160805': 0, '20160806': 1, '20160807': 1, '20160808': 0, '20160809': 0, '20160810': 0, '20160811': 0, '20160812': 0, '20160813': 1, '20160814': 1, '20160815': 0, '20160816': 0, '20160817': 0, '20160818': 0, '20160819': 0, '20160820': 1, '20160821': 1, '20160822': 0, '20160823': 0, '20160824': 0, '20160825': 0, '20160826': 0, '20160827': 1, '20160828': 1, '20160829': 0, '20160830': 0, '20160831': 0}, '201610': {'20161001': 2, '20161002': 2, '20161003': 2, '20161004': 2, '20161005': 2, '20161006': 2, '20161007': 2, '20161008': 0, '20161009': 0, '20161010': 0, '20161011': 0, '20161012': 0, '20161013': 0, '20161014': 0, '20161015': 1, '20161016': 1, '20161017': 0, '20161018': 0, '20161019': 0, '20161020': 0, '20161021': 0, '20161022': 1, '20161023': 1, '20161024': 0, '20161025': 0, '20161026': 0, '20161027': 0, '20161028': 0, '20161029': 1, '20161030': 1, '20161031': 0}, '201611': {'20161101': 0, '20161102': 0, '20161103': 0, '20161104': 0, '20161105': 1, '20161106': 1, '20161107': 0, '20161108': 0, '20161109': 0, '20161110': 0, '20161111': 0, '20161112': 1, '20161113': 1, '20161114': 0, '20161115': 0, '20161116': 0, '20161117': 0, '20161118': 0, '20161119': 1, '20161120': 1, '20161121': 0, '20161122': 0, '20161123': 0, '20161124': 0, '20161125': 0, '20161126': 1, '20161127': 1, '20161128': 0, '20161129': 0, '20161130': 0}, '201612': {'20161201': 0, '20161202': 0, '20161203': 1, '20161204': 1, '20161205': 0, '20161206': 0, '20161207': 0, '20161208': 0, '20161209': 0, '20161210': 1, '20161211': 1, '20161212': 0, '20161213': 0, '20161214': 0, '20161215': 0, '20161216': 0, '20161217': 1, '20161218': 1, '20161219': 0, '20161220': 0, '20161221': 0, '20161222': 0, '20161223': 0, '20161224': 1, '20161225': 1, '20161226': 0, '20161227': 0, '20161228': 0, '20161229': 0, '20161230': 0, '20161231': 1}}
只等查 2018、2017 和 2016 年的节假日
None
爬取地址: http://holidays-calendar.net/2017/calendar_zh_cn/china_zh_cn.html
{'20170801': 0, '20170802': 0, '20170803': 0, '20170804': 0, '20170805': 1, '20170806': 1, '20170807': 0, '20170808': 0, '20170809': 0, '20170810': 0, '20170811': 0, '20170812': 1, '20170813': 1, '20170814': 0, '20170815': 0, '20170816': 0, '20170817': 0, '20170818': 0, '20170819': 1, '20170820': 1, '20170821': 0, '20170822': 0, '20170823': 0, '20170824': 0, '20170825': 0, '20170826': 1, '20170827': 1, '20170828': 0, '20170829': 0, '20170830': 0, '20170831': 0}
爬取地址: http://holidays-calendar.net/2017/calendar_zh_cn/china_zh_cn.html
2
```

