[General]
# warning, notify, info, verbose
skip-proxy = 192.168.0.0/16, 10.0.0.0/8, 172.16.0.0/12, 100.64.0.0/10, localhost, *.local,e.crashlytics.com
bypass-tun = 0.0.0.0/8, 192.168.0.0/16, 10.0.0.0/8, 172.16.0.0/12, 100.64.0.0/10
loglevel = notify
# dns-server = 223.5.5.5,223.6.6.6,114.114.114.114,114.114.115.115

[Proxy]
💊 Play with GFW = direct
🇯🇵 JP = custom,1.2.3.4,443,rc4-md5,password,http://custom/ss.module
🇺🇸 US = custom <<<

[Proxy Group]
Proxy = select, 💊 Play with GFW, 🇯🇵 JP,🇺🇸US

[Rule]
# Some services are available locally
DOMAIN-KEYWORD,aka,Proxy
DOMAIN-SUFFIX,ccgslb.com,DIRECT
DOMAIN-SUFFIX,ccgslb.net,DIRECT
DOMAIN-SUFFIX,edu.cn,DIRECT
DOMAIN-SUFFIX,ourdvs.com,DIRECT
DOMAIN-SUFFIX,ls.apple.com,DIRECT
DOMAIN-SUFFIX,dl.google.com,DIRECT

# Apple
DOMAIN-SUFFIX,adcdownload.apple.com,DIRECT
DOMAIN-SUFFIX,appldnld.apple.com,DIRECT
DOMAIN-SUFFIX,cdn-apple.com,DIRECT
DOMAIN-SUFFIX,icloud-content.com,Proxy
DOMAIN-SUFFIX,icloud.com,Proxy
DOMAIN-SUFFIX,itunes.com,Proxy
DOMAIN-SUFFIX,lcdn-registration.apple.com,DIRECT
DOMAIN-SUFFIX,ls.apple.com,DIRECT
DOMAIN-SUFFIX,mzstatic.com,DIRECT
DOMAIN-SUFFIX,swcdn.apple.com,DIRECT

DOMAIN,aod.itunes.apple.com,DIRECT
DOMAIN,bookkeeper.itunes.apple.com,DIRECT
DOMAIN,client-api.itunes.apple.com,DIRECT
DOMAIN,init.itunes.apple.com,DIRECT
DOMAIN,itunes.apple.com,DIRECT
DOMAIN,iosapps.itunes.apple.com,DIRECT
DOMAIN,osxapps.itunes.apple.com,DIRECT
DOMAIN,pd-st.itunes.apple.com,DIRECT
DOMAIN,play.itunes.apple.com,DIRECT
DOMAIN,se.itunes.apple.com,DIRECT
DOMAIN,sp.itunes.apple.com,DIRECT
DOMAIN,streamingaudio.itunes.apple.com,DIRECT
DOMAIN,su.itunes.apple.com,DIRECT
DOMAIN,upp.itunes.apple.com,DIRECT

DOMAIN-SUFFIX,apple.com,Proxy
DOMAIN-SUFFIX,apple.co,Proxy

# Baidu
DOMAIN-SUFFIX,baidupcs.com,DIRECT
DOMAIN-SUFFIX,hiphotos.baidu.com,DIRECT
DOMAIN-SUFFIX,img.baidu.com,DIRECT
DOMAIN-SUFFIX,timg.baidu.com,DIRECT
DOMAIN-SUFFIX,map.baidu.com,DIRECT
DOMAIN-SUFFIX,pan.baidu.com,DIRECT
DOMAIN-SUFFIX,pcs.baidu.com,DIRECT
DOMAIN-SUFFIX,passport.baidu.com,DIRECT
DOMAIN-SUFFIX,waimai.baidu.com,DIRECT
DOMAIN-SUFFIX,yun.baidu.com,DIRECT
DOMAIN-SUFFIX,tieba.baidu.com,DIRECT

# QQ
DOMAIN-SUFFIX,beacon.qq.com,REJECT
DOMAIN-SUFFIX,monitor.uu.qq.com,REJECT
DOMAIN-SUFFIX,pgdt.gtimg.cn,REJECT
DOMAIN-SUFFIX,pingjs.qq.com,REJECT
DOMAIN-SUFFIX,pingtcss.qq.com,REJECT
DOMAIN-SUFFIX,report.qq.com,REJECT
DOMAIN-SUFFIX,tajs.qq.com,REJECT
DOMAIN-SUFFIX,tcss.qq.com,REJECT

# Block privacy tracker within apps
DOMAIN,ads.mopub.com,REJECT
DOMAIN,cpro.baidu.com,REJECT
DOMAIN,hmma.baidu.com,REJECT
DOMAIN,monitor.uu.qq.com,REJECT
DOMAIN,pagead2.googlesyndication.com,REJECT
DOMAIN,pingma.qq.com,REJECT
DOMAIN,stat.m.jd.com,REJECT
DOMAIN-KEYWORD,cnzz,REJECT
DOMAIN-KEYWORD,analytics.,REJECT
DOMAIN-KEYWORD,flurry.co,REJECT
DOMAIN-KEYWORD,umeng.co,REJECT
DOMAIN-SUFFIX,127.net,REJECT
DOMAIN-SUFFIX,applovin.com,REJECT
DOMAIN-SUFFIX,doubleclick.net,REJECT
DOMAIN-SUFFIX,mmstat.com,REJECT
DOMAIN-SUFFIX,mob.com,REJECT
DOMAIN-SUFFIX,sponsorpay.com,REJECT
DOMAIN-SUFFIX,youmi.net,REJECT

# Disable customized fonts
DOMAIN,fonts.googleapis.com,REJECT

# Prevent sniffer from a public WiFi
DOMAIN,init.icloud-analysis.com,REJECT

# AD Block
DOMAIN-KEYWORD,admaster,REJECT
DOMAIN-KEYWORD,adsage,REJECT
DOMAIN-KEYWORD,adsmogo,REJECT
DOMAIN-KEYWORD,adsrvmedia,REJECT
DOMAIN-KEYWORD,analytics,REJECT
DOMAIN-KEYWORD,clkservice,REJECT
DOMAIN-KEYWORD,cnzz,REJECT
DOMAIN-KEYWORD,counter,REJECT
DOMAIN-KEYWORD,domob,REJECT
DOMAIN-KEYWORD,duomeng,REJECT
DOMAIN-KEYWORD,feedback,REJECT
DOMAIN-KEYWORD,float,REJECT
DOMAIN-KEYWORD,googleads,REJECT
DOMAIN-KEYWORD,openx,REJECT
DOMAIN-KEYWORD,pagead2,REJECT
DOMAIN-KEYWORD,tongji,REJECT
DOMAIN-KEYWORD,umeng,REJECT
DOMAIN-KEYWORD,usage,REJECT

DOMAIN-SUFFIX,10up.com,REJECT
DOMAIN-SUFFIX,51.la,REJECT
DOMAIN-SUFFIX,58.com,REJECT
DOMAIN-SUFFIX,58cdn.com.cn,REJECT
DOMAIN-SUFFIX,99click.com,REJECT
DOMAIN-SUFFIX,acjs.aliyun.com,REJECT
DOMAIN-SUFFIX,acs86.com,REJECT
DOMAIN-SUFFIX,ad.3.cn,REJECT
DOMAIN-SUFFIX,ad.thepaper.cn,REJECT
DOMAIN-SUFFIX,ad.unimhk.com,REJECT
DOMAIN-SUFFIX,adbxb.com,REJECT
DOMAIN-SUFFIX,adchina.com,REJECT
DOMAIN-SUFFIX,adcome.cn,REJECT
DOMAIN-SUFFIX,adform.net,REJECT
DOMAIN-SUFFIX,adinfuse.com,REJECT
DOMAIN-SUFFIX,adjust.com,REJECT
DOMAIN-SUFFIX,adjust.io,REJECT
DOMAIN-SUFFIX,adlive.cn,REJECT
DOMAIN-SUFFIX,adm.easou.com,REJECT
DOMAIN-SUFFIX,admin5.com,REJECT
DOMAIN-SUFFIX,admob.com,REJECT
DOMAIN-SUFFIX,admon.cn,REJECT
DOMAIN-SUFFIX,adnxs.com,REJECT
DOMAIN-SUFFIX,ads.feedly.com,REJECT
DOMAIN-SUFFIX,ads.genieessp.com,REJECT
DOMAIN-SUFFIX,ads.mobclix.com,REJECT
DOMAIN-SUFFIX,ads.yahoo.com,REJECT
DOMAIN-SUFFIX,adsame.com,REJECT
DOMAIN-SUFFIX,aduu.cn,REJECT
DOMAIN-SUFFIX,adview.cn,REJECT
DOMAIN-SUFFIX,adwhirl.com,REJECT
DOMAIN-SUFFIX,adwo.com,REJECT
DOMAIN-SUFFIX,adxmi.com,REJECT
DOMAIN-SUFFIX,adzerk.net,REJECT
DOMAIN-SUFFIX,allyes.com,REJECT
DOMAIN-SUFFIX,anquan.org,REJECT
DOMAIN-SUFFIX,aoodoo.feng.com,REJECT
DOMAIN-SUFFIX,api.mobile.dianru.com,REJECT
DOMAIN-SUFFIX,appads.com,REJECT
DOMAIN-SUFFIX,appboy.com,REJECT
DOMAIN-SUFFIX,applifier.com,REJECT
DOMAIN-SUFFIX,applovin.com,REJECT
DOMAIN-SUFFIX,appsflyer.com,REJECT
DOMAIN-SUFFIX,atdmt.com,REJECT
DOMAIN-SUFFIX,baifendian.com,REJECT
DOMAIN-SUFFIX,bam.nr-data.net,REJECT
DOMAIN-SUFFIX,baycode.cn,REJECT
DOMAIN-SUFFIX,beacon.sina.com.cn,REJECT
DOMAIN-SUFFIX,beacon.tingyun.com,REJECT
DOMAIN-SUFFIX,chance-ad.com,REJECT
DOMAIN-SUFFIX,chartboost.com,REJECT
DOMAIN-SUFFIX,clicktracks.com,REJECT
DOMAIN-SUFFIX,clickzs.com,REJECT
DOMAIN-SUFFIX,cm.ipinyou.com,REJECT
DOMAIN-SUFFIX,cmcore.com,REJECT
DOMAIN-SUFFIX,coremetrics.com,REJECT
DOMAIN-SUFFIX,cps.360buy.com,REJECT
DOMAIN-SUFFIX,cpro.baidustatic.com,REJECT
DOMAIN-SUFFIX,dsp.youdao.com,REJECT
DOMAIN-SUFFIX,emarbox.com,REJECT
DOMAIN-SUFFIX,fastapi.net,REJECT
DOMAIN-SUFFIX,fastclick.net,REJECT
DOMAIN-SUFFIX,fengbuy.com,REJECT
DOMAIN-SUFFIX,geetest.com,REJECT
DOMAIN-SUFFIX,guohead.com,REJECT
DOMAIN-SUFFIX,guomob.com,REJECT
DOMAIN-SUFFIX,hydra.alibaba.com,REJECT
DOMAIN-SUFFIX,ib.adnxs.com,REJECT
DOMAIN-SUFFIX,immob.cn,REJECT
DOMAIN-SUFFIX,inmobi.com,REJECT
DOMAIN-SUFFIX,istreamsche.com,REJECT
DOMAIN-SUFFIX,jusha.com,REJECT
DOMAIN-SUFFIX,kouyu.youdao.com,REJECT
DOMAIN-SUFFIX,lotuseed.com,REJECT
DOMAIN-SUFFIX,lu.com,REJECT
DOMAIN-SUFFIX,lufax.com,REJECT
DOMAIN-SUFFIX,m.simaba.taobao.com,REJECT
DOMAIN-SUFFIX,madmini.com,REJECT
DOMAIN-SUFFIX,mediav.com,REJECT
DOMAIN-SUFFIX,miaozhen.com,REJECT
DOMAIN-SUFFIX,miidi.net,REJECT
DOMAIN-SUFFIX,mixpanel.com,REJECT
DOMAIN-SUFFIX,mng-ads.com,REJECT
DOMAIN-SUFFIX,mobfox.com,REJECT
DOMAIN-SUFFIX,mobisage.cn,REJECT
DOMAIN-SUFFIX,mobileapptracking.com,REJECT
DOMAIN-SUFFIX,mopub.com,REJECT
DOMAIN-SUFFIX,mxpnl.com,REJECT
DOMAIN-SUFFIX,networkbench.com,REJECT
DOMAIN-SUFFIX,newrelic.com,REJECT
DOMAIN-SUFFIX,ntalker.com,REJECT
DOMAIN-SUFFIX,o2omobi.com,REJECT
DOMAIN-SUFFIX,oadz.com,REJECT
DOMAIN-SUFFIX,oneapm.com,REJECT
DOMAIN-SUFFIX,optimizely.com,REJECT
DOMAIN-SUFFIX,overture.com,REJECT
DOMAIN-SUFFIX,page.amap.com,REJECT
DOMAIN-SUFFIX,pubnub.com,REJECT
DOMAIN-SUFFIX,qtmojo.com,REJECT
DOMAIN-SUFFIX,reachmax.cn,REJECT
DOMAIN-SUFFIX,responsys.net,REJECT
DOMAIN-SUFFIX,rollout.io,REJECT
DOMAIN-SUFFIX,sandai.net,REJECT
DOMAIN-SUFFIX,sax.sina.cn,REJECT
DOMAIN-SUFFIX,sax.sina.com.cn,REJECT
DOMAIN-SUFFIX,scorecardresearch.com,REJECT
DOMAIN-SUFFIX,serving-sys.com,REJECT
DOMAIN-SUFFIX,sitemeter.com,REJECT
DOMAIN-SUFFIX,smartmad.com,REJECT
DOMAIN-SUFFIX,sponsorpay.com,REJECT
DOMAIN-SUFFIX,statcounter.com,REJECT
DOMAIN-SUFFIX,sysdig.com,REJECT
DOMAIN-SUFFIX,tanx.com,REJECT
DOMAIN-SUFFIX,tapjoyads.com,REJECT
DOMAIN-SUFFIX,tdimg.com,REJECT
DOMAIN-SUFFIX,tjlog.easou.com,REJECT
DOMAIN-SUFFIX,tjlog.ps.easou.com,REJECT
DOMAIN-SUFFIX,tjs.sjs.sinajs.cn,REJECT
DOMAIN-SUFFIX,trafficmp.com,REJECT
DOMAIN-SUFFIX,umtrack.com,REJECT
DOMAIN-SUFFIX,union.youdao.com,REJECT
DOMAIN-SUFFIX,unlitui.com,REJECT
DOMAIN-SUFFIX,ushaqi.com,REJECT
DOMAIN-SUFFIX,uyunad.com,REJECT
DOMAIN-SUFFIX,vamaker.com,REJECT
DOMAIN-SUFFIX,vpon.com,REJECT
DOMAIN-SUFFIX,wanproxy.127.net,REJECT
DOMAIN-SUFFIX,wiyun.com,REJECT
DOMAIN-SUFFIX,wooboo.com.cn,REJECT
DOMAIN-SUFFIX,wqmobile.com,REJECT
DOMAIN-SUFFIX,wrating.com,REJECT
DOMAIN-SUFFIX,ws.126.net,REJECT
DOMAIN-SUFFIX,xiaozhen.com,REJECT
DOMAIN-SUFFIX,xibao100.com,REJECT
DOMAIN-SUFFIX,yes1.feng.com,REJECT
DOMAIN-SUFFIX,yiqifa.com,REJECT
DOMAIN-SUFFIX,youmi.net,REJECT
DOMAIN-SUFFIX,zhstatic.zhihu.com,REJECT

# Force some domains which are fucked by GFW while resolving DNS
DOMAIN-KEYWORD,blogspot,Proxy,force-remote-dns
DOMAIN-KEYWORD,facebook,Proxy,force-remote-dns
DOMAIN-KEYWORD,gmail,Proxy,force-remote-dns
DOMAIN-KEYWORD,google,Proxy,force-remote-dns
DOMAIN-KEYWORD,instagram,Proxy,force-remote-dns
DOMAIN-KEYWORD,jackd,Proxy,force-remote-dns
DOMAIN-KEYWORD,twitter,Proxy,force-remote-dns
DOMAIN-KEYWORD,youtube,Proxy,force-remote-dns
DOMAIN-SUFFIX,t.co,Proxy,force-remote-dns
DOMAIN-SUFFIX,twimg.com,Proxy,force-remote-dns
DOMAIN-SUFFIX,kenengba.com,Proxy,force-remote-dns

# Accelerate .cn sites
DOMAIN-SUFFIX,cn,DIRECT
DOMAIN-KEYWORD,cn.img,DIRECT
DOMAIN-KEYWORD,cn.service,DIRECT
DOMAIN-KEYWORD,360buy,DIRECT
DOMAIN-KEYWORD,alipay,DIRECT
DOMAIN-KEYWORD,baidu,DIRECT
DOMAIN-KEYWORD,taobao,DIRECT
DOMAIN-KEYWORD,zh-cn,DIRECT

DOMAIN-SUFFIX,126.net,DIRECT
DOMAIN-SUFFIX,163.com,DIRECT
DOMAIN-SUFFIX,36kr.com,DIRECT
DOMAIN-SUFFIX,acfun.tv,DIRECT
DOMAIN-SUFFIX,acgvideo.com,DIRECT
DOMAIN-SUFFIX,aixifan.com,DIRECT
DOMAIN-SUFFIX,alicdn.com,DIRECT
DOMAIN-SUFFIX,amap.com,DIRECT
DOMAIN-SUFFIX,bababian.com,DIRECT
DOMAIN-SUFFIX,bdimg.com,DIRECT
DOMAIN-SUFFIX,bdstatic.com,DIRECT
DOMAIN-SUFFIX,bilibili.com,DIRECT
DOMAIN-SUFFIX,bing.com,DIRECT
DOMAIN-SUFFIX,caiyunapp.com,DIRECT
DOMAIN-SUFFIX,chinacache.net,DIRECT
DOMAIN-SUFFIX,clouddn.com,DIRECT
DOMAIN-SUFFIX,cnbeta.com,DIRECT
DOMAIN-SUFFIX,cnbetacdn.com,DIRECT
DOMAIN-SUFFIX,douban.com,DIRECT
DOMAIN-SUFFIX,doubanio.com,DIRECT
DOMAIN-SUFFIX,duokan.com,DIRECT
DOMAIN-SUFFIX,easou.com,DIRECT
DOMAIN-SUFFIX,bbs.feng.com,DIRECT
DOMAIN-SUFFIX,fresh-ideas.cc,DIRECT
DOMAIN-SUFFIX,fir.im,DIRECT
DOMAIN-SUFFIX,frdic.com,DIRECT
DOMAIN-SUFFIX,godic.net,DIRECT
DOMAIN-SUFFIX,gtimg.com,DIRECT
DOMAIN-SUFFIX,hao123.com,DIRECT
DOMAIN-SUFFIX,haosou.com,DIRECT
DOMAIN-SUFFIX,hdslb.com,DIRECT
DOMAIN-SUFFIX,hdslb.net,DIRECT
DOMAIN-SUFFIX,iciba.com,DIRECT
DOMAIN-SUFFIX,ifeng.com,DIRECT
DOMAIN-SUFFIX,ifengimg.com,DIRECT
DOMAIN-SUFFIX,iqiyi.com,DIRECT
DOMAIN-SUFFIX,jd.com,DIRECT
DOMAIN-SUFFIX,jianshu.com,DIRECT
DOMAIN-SUFFIX,jianshu.io,DIRECT
DOMAIN-SUFFIX,jianshuapi.com,DIRECT
DOMAIN-SUFFIX,luoo.net,DIRECT
DOMAIN-SUFFIX,mi.com,DIRECT
DOMAIN-SUFFIX,microsoft.com,DIRECT
DOMAIN-SUFFIX,miaopai.com,DIRECT
DOMAIN-SUFFIX,moke.com,DIRECT
DOMAIN-SUFFIX,netease.com,DIRECT
DOMAIN-SUFFIX,pstatp.com,DIRECT
DOMAIN-SUFFIX,qhimg.com,DIRECT
DOMAIN-SUFFIX,qiniucdn.com,DIRECT
DOMAIN-SUFFIX,qiniudn.com,DIRECT
DOMAIN-SUFFIX,qq.com,DIRECT
DOMAIN-SUFFIX,qqurl.com,DIRECT
DOMAIN-SUFFIX,ruguoapp.com,DIRECT
DOMAIN-SUFFIX,sinaapp.com,DIRECT
DOMAIN-SUFFIX,snwx.com,DIRECT
DOMAIN-SUFFIX,sogou.com,DIRECT
DOMAIN-SUFFIX,sohu.com,DIRECT
DOMAIN-SUFFIX,soso.com,DIRECT
DOMAIN-SUFFIX,sspai.com,DIRECT
DOMAIN-SUFFIX,suning.com,DIRECT
DOMAIN-SUFFIX,tenpay.com,DIRECT
DOMAIN-SUFFIX,tietuku.com,DIRECT
DOMAIN-SUFFIX,tmall.com,DIRECT
DOMAIN-SUFFIX,tudou.com,DIRECT
DOMAIN-SUFFIX,upaiyun.com,DIRECT
DOMAIN-SUFFIX,uxengine.net,DIRECT
DOMAIN-SUFFIX,v2ex.co,DIRECT
DOMAIN-SUFFIX,v2ex.com,DIRECT
DOMAIN-SUFFIX,weibo.com,DIRECT
DOMAIN-SUFFIX,weiphone.net,DIRECT
DOMAIN-SUFFIX,weiphone.com,DIRECT
DOMAIN-SUFFIX,windowsupdate.com,DIRECT
DOMAIN-SUFFIX,xiami.com,DIRECT
DOMAIN-SUFFIX,xiami.net,DIRECT
DOMAIN-SUFFIX,xiaomi.com,DIRECT
DOMAIN-SUFFIX,xiaomi.net,DIRECT
DOMAIN-SUFFIX,xitek.com,DIRECT
DOMAIN-SUFFIX,xunlei.com,DIRECT
DOMAIN-SUFFIX,yhd.com,DIRECT
DOMAIN-SUFFIX,yinxiang.com,DIRECT
DOMAIN-SUFFIX,yixia.com,DIRECT
DOMAIN-SUFFIX,youku.com,DIRECT
DOMAIN-SUFFIX,zhihu.com,DIRECT
DOMAIN-SUFFIX,zhimg.com,DIRECT

# Top blocked sites
DOMAIN-KEYWORD,amazon,Proxy
DOMAIN-KEYWORD,appledaily,Proxy
DOMAIN-KEYWORD,blogspot,Proxy
DOMAIN-KEYWORD,dropbox,Proxy

DOMAIN-SUFFIX,4sqi.net,Proxy
DOMAIN-SUFFIX,9to5mac.com,Proxy
DOMAIN-SUFFIX,aerisapi.com,Proxy
DOMAIN-SUFFIX,alfredapp.com,Proxy
DOMAIN-SUFFIX,amplitude.com,Proxy
DOMAIN-SUFFIX,android.com,Proxy
DOMAIN-SUFFIX,angularjs.org,Proxy
DOMAIN-SUFFIX,apple-dns.net,Proxy
DOMAIN-SUFFIX,appspot.com,Proxy
DOMAIN-SUFFIX,att.com,Proxy
DOMAIN-SUFFIX,azurewebsites.net,Proxy
DOMAIN-SUFFIX,bit.ly,Proxy
DOMAIN-SUFFIX,bitbucket.org,Proxy
DOMAIN-SUFFIX,blog.com,Proxy
DOMAIN-SUFFIX,blogcdn.com,Proxy
DOMAIN-SUFFIX,blogger.com,Proxy
DOMAIN-SUFFIX,blogsmithmedia.com,Proxy
DOMAIN-SUFFIX,bloomberg.com,Proxy
DOMAIN-SUFFIX,box.net,Proxy
DOMAIN-SUFFIX,cachefly.net,Proxy
DOMAIN-SUFFIX,chromium.org,Proxy
DOMAIN-SUFFIX,cl.ly,Proxy
DOMAIN-SUFFIX,cloudflare.com,Proxy
DOMAIN-SUFFIX,cloudfront.net,Proxy
DOMAIN-SUFFIX,cloudmagic.com,Proxy
DOMAIN-SUFFIX,cocoapods.org,Proxy
DOMAIN-SUFFIX,crashlytics.com,Proxy
DOMAIN-SUFFIX,d.pr,Proxy
DOMAIN-SUFFIX,dayone.me,Proxy
DOMAIN-SUFFIX,droplr.com,Proxy
DOMAIN-SUFFIX,digicert.com,Proxy
DOMAIN-SUFFIX,dnsimple.com,Proxy
DOMAIN-SUFFIX,docker.com,Proxy
DOMAIN-SUFFIX,dribbble.com,Proxy
DOMAIN-SUFFIX,duckduckgo.com,Proxy
DOMAIN-SUFFIX,edgecastcdn.net,Proxy
DOMAIN-SUFFIX,edgesuite.net,Proxy
DOMAIN-SUFFIX,engadget.com,Proxy
DOMAIN-SUFFIX,eurekavpt.com,Proxy
DOMAIN-SUFFIX,evernote.com,Proxy
DOMAIN-SUFFIX,fabric.io,Proxy
DOMAIN-SUFFIX,fastly.net,Proxy
DOMAIN-SUFFIX,fb.me,Proxy
DOMAIN-SUFFIX,fbcdn.net,Proxy
DOMAIN-SUFFIX,fc2.com,Proxy
DOMAIN-SUFFIX,feedburner.com,Proxy
DOMAIN-SUFFIX,feedly.com,Proxy
DOMAIN-SUFFIX,feedsportal.com,Proxy
DOMAIN-SUFFIX,flickr.com,Proxy
DOMAIN-SUFFIX,g.co,Proxy
DOMAIN-SUFFIX,ggpht.com,Proxy
DOMAIN-SUFFIX,git.io,Proxy
DOMAIN-SUFFIX,github.com,Proxy
DOMAIN-SUFFIX,githubapp.com,Proxy
DOMAIN-SUFFIX,github.io,Proxy
DOMAIN-SUFFIX,githubusercontent.com,Proxy
DOMAIN-SUFFIX,godaddy.com,Proxy
DOMAIN-SUFFIX,golang.org,Proxy
DOMAIN-SUFFIX,goo.gl,Proxy
DOMAIN-SUFFIX,goodreaders.com,Proxy
DOMAIN-SUFFIX,goodreads.com,Proxy
DOMAIN-SUFFIX,gravatar.com,Proxy
DOMAIN-SUFFIX,gstatic.com,Proxy
DOMAIN-SUFFIX,icons8.com,Proxy
DOMAIN-SUFFIX,ift.tt,Proxy
DOMAIN-SUFFIX,imageshack.us,Proxy
DOMAIN-SUFFIX,img.ly,Proxy
DOMAIN-SUFFIX,imgur.com,Proxy
DOMAIN-SUFFIX,instapaper.com,Proxy
DOMAIN-SUFFIX,ipn.li,Proxy
DOMAIN-SUFFIX,is.gd,Proxy
DOMAIN-SUFFIX,itun.es,Proxy
DOMAIN-SUFFIX,j.mp,Proxy
DOMAIN-SUFFIX,jshint.com,Proxy
DOMAIN-SUFFIX,kat.cr,Proxy
DOMAIN-SUFFIX,libsyn.com,Proxy
DOMAIN-SUFFIX,licdn.com,Proxy
DOMAIN-SUFFIX,linkedin.com,Proxy
DOMAIN-SUFFIX,linode.com,Proxy
DOMAIN-SUFFIX,lithium.com,Proxy
DOMAIN-SUFFIX,live.com,Proxy
DOMAIN-SUFFIX,live.net,Proxy
DOMAIN-SUFFIX,livefilestore.com,Proxy
DOMAIN-SUFFIX,mathjax.org,Proxy
DOMAIN-SUFFIX,medium.com,Proxy
DOMAIN-SUFFIX,megaupload.com,Proxy
DOMAIN-SUFFIX,mobile01.com,Proxy
DOMAIN-SUFFIX,modmyi.com,Proxy
DOMAIN-SUFFIX,msedge.net,Proxy
DOMAIN-SUFFIX,name.com,Proxy
DOMAIN-SUFFIX,nextmedia.com,Proxy
DOMAIN-SUFFIX,nyt.com,Proxy
DOMAIN-SUFFIX,nytimes.com,Proxy
DOMAIN-SUFFIX,office365.com,Proxy
DOMAIN-SUFFIX,omnigroup.com,Proxy
DOMAIN-SUFFIX,onenote.com,Proxy
DOMAIN-SUFFIX,openvpn.net,Proxy
DOMAIN-SUFFIX,openwrt.org,Proxy
DOMAIN-SUFFIX,outlook.com,Proxy
DOMAIN-SUFFIX,ow.ly,Proxy
DOMAIN-SUFFIX,parallels.com,Proxy
DOMAIN-SUFFIX,periscope.tv,Proxy
DOMAIN-SUFFIX,playpcesor.com,Proxy
DOMAIN-SUFFIX,pinboard.in,Proxy
DOMAIN-SUFFIX,qdaily.com,Proxy
DOMAIN-SUFFIX,scdn.co,Proxy
DOMAIN-SUFFIX,skype.com,Proxy
DOMAIN-SUFFIX,smartmailcloud.com,Proxy
DOMAIN-SUFFIX,sndcdn.com,Proxy
DOMAIN-SUFFIX,soundcloud.com,Proxy
DOMAIN-SUFFIX,spotify.com,Proxy
DOMAIN-SUFFIX,squarespace.com,Proxy
DOMAIN-SUFFIX,sstatic.net,Proxy
DOMAIN-SUFFIX,stackoverflow.com,Proxy
DOMAIN-SUFFIX,staticflickr.com,Proxy
DOMAIN-SUFFIX,symauth.com,Proxy
DOMAIN-SUFFIX,symcb.com,Proxy
DOMAIN-SUFFIX,symcd.com,Proxy
DOMAIN-SUFFIX,tapbots.com,Proxy
DOMAIN-SUFFIX,tapbots.net,Proxy
DOMAIN-SUFFIX,tdesktop.com,Proxy
DOMAIN-SUFFIX,techcrunch.com,Proxy
DOMAIN-SUFFIX,thepiratebay.org,Proxy
DOMAIN-SUFFIX,tiny.cc,Proxy
DOMAIN-SUFFIX,tinypic.com,Proxy
DOMAIN-SUFFIX,tmblr.co,Proxy
DOMAIN-SUFFIX,trello.com,Proxy
DOMAIN-SUFFIX,tumblr.com,Proxy
DOMAIN-SUFFIX,twitch.tv,Proxy
DOMAIN-SUFFIX,txmblr.com,Proxy
DOMAIN-SUFFIX,typekit.net,Proxy
DOMAIN-SUFFIX,ubnt.com,Proxy
DOMAIN-SUFFIX,urchin.com,Proxy
DOMAIN-SUFFIX,v.gd,Proxy
DOMAIN-SUFFIX,vimeo.com,Proxy
DOMAIN-SUFFIX,vine.co,Proxy
DOMAIN-SUFFIX,vsco.co,Proxy
DOMAIN-SUFFIX,weather.com,Proxy
DOMAIN-SUFFIX,wikimedia.org,Proxy
DOMAIN-SUFFIX,wikipedia.com,Proxy
DOMAIN-SUFFIX,wikipedia.org,Proxy
DOMAIN-SUFFIX,windows.net,Proxy
DOMAIN-SUFFIX,wordpress.com,Proxy
DOMAIN-SUFFIX,wp.com,Proxy
DOMAIN-SUFFIX,wsj.com,Proxy
DOMAIN-SUFFIX,wsj.net,Proxy
DOMAIN-SUFFIX,yahoo.com,Proxy
DOMAIN-SUFFIX,youtu.be,Proxy
DOMAIN-SUFFIX,ytimg.com,Proxy

# Ads in Video apps
DOMAIN-SUFFIX,ad.api.3g.tudou.com,REJECT
DOMAIN-SUFFIX,ad.api.3g.youku.com,REJECT
DOMAIN-SUFFIX,ad.m.iqiyi.com,REJECT
DOMAIN-SUFFIX,adcontrol.tudou.com,REJECT
DOMAIN-SUFFIX,adplay.tudou.com,REJECT
DOMAIN-SUFFIX,afp.qiyi.com,REJECT
DOMAIN-SUFFIX,agn.aty.sohu.com,REJECT
DOMAIN-SUFFIX,ark.letv.com,REJECT
DOMAIN-SUFFIX,asimgs.pplive.cn,REJECT
DOMAIN-SUFFIX,atm.youku.com,REJECT
DOMAIN-SUFFIX,cupid.iqiyi.com,REJECT
DOMAIN-SUFFIX,cupid.qiyi.com,REJECT
DOMAIN-SUFFIX,de.as.pptv.com,REJECT
DOMAIN-SUFFIX,g.uusee.com,REJECT
DOMAIN-SUFFIX,ifacelog.iqiyi.com,REJECT
DOMAIN-SUFFIX,iwstat.tudou.com,REJECT
DOMAIN-SUFFIX,lives.l.qq.com,REJECT
DOMAIN-SUFFIX,logstat.t.sfht.com,REJECT
DOMAIN-SUFFIX,lstat.youku.com,REJECT
DOMAIN-SUFFIX,m.aty.sohu.com,REJECT
DOMAIN-SUFFIX,n.mark.letv.com,REJECT
DOMAIN-SUFFIX,nstat.tudou.com,REJECT
DOMAIN-SUFFIX,pop.uusee.com,REJECT
DOMAIN-SUFFIX,rcd.iqiyi.com,REJECT
DOMAIN-SUFFIX,stat.tudou.com,REJECT
DOMAIN-SUFFIX,stat.youku.com,REJECT
DOMAIN-SUFFIX,static.g.ppstream.com,REJECT
DOMAIN-SUFFIX,static.lstat.youku.com,REJECT
DOMAIN-SUFFIX,static.qiyi.com,REJECT
DOMAIN-SUFFIX,stats.tudou.com,REJECT
DOMAIN-SUFFIX,traffic.uusee.com,REJECT
IP-CIDR,123.125.117.0/22,REJECT,no-resolve

# Beijing Mobile Float
IP-CIDR,221.179.140.145/32,REJECT,no-resolve
# ShangHai Unicom Float
IP-CIDR,220.196.52.141/32,REJECT,no-resolve
# Jiangsu Telecom Float
IP-CIDR,221.228.17.152/32,REJECT,no-resolve
# WuHan Telecom Float
IP-CIDR,111.175.220.160/29,REJECT,no-resolve
# Wuhan Unicom Float
IP-CIDR,113.57.230.88/32,REJECT,no-resolve
# HangZhou Unicom Float
IP-CIDR,124.160.194.11/32,REJECT,no-resolve

# Telegram
IP-CIDR,91.108.56.0/22,Proxy,no-resolve
IP-CIDR,91.108.4.0/22,Proxy,no-resolve
IP-CIDR,109.239.140.0/24,Proxy,no-resolve
IP-CIDR,149.154.160.0/20,Proxy,no-resolve

# LAN
IP-CIDR,192.168.0.0/16,DIRECT
IP-CIDR,10.0.0.0/8,DIRECT
IP-CIDR,100.64.0.0/10, DIRECT
IP-CIDR,172.16.0.0/12,DIRECT
IP-CIDR,127.0.0.0/8,DIRECT

GEOIP,CN,DIRECT
FINAL,Proxy

[Host]
# Chengdu Apple DNS
iosapps.itunes.apple.com = 182.140.218.60
streamingaudio.itunes.apple.com = 182.140.218.60
aod.itunes.apple.com = 182.140.218.60
radio.itunes.apple.com = 184.87.100.246
radio-services.itunes.apple.com = 184.87.100.246
radio-activity.itunes.apple.com = 184.87.100.246
search.itunes.apple.com = 184.87.97.50
play.itunes.apple.com = 118.123.106.105
upp.itunes.apple.com = 118.123.106.105
client-api.itunes.apple.com = 118.123.106.105
