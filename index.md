## BurpSuite Highlighter and Extractor

HaE is used to highlight HTTP requests and extract information from `HTTP response messages` or `request messages`.

## Public Rules

Copy to `config.json`

```json
{
    "Fingerprint: 金蝶EAS": {
        "loaded": true,
        "regex": "(easSessionId)",
        "color": "gray",
        "engine": "dfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: H3C AM8000": {
        "loaded": true,
        "regex": "(AM8000)",
        "color": "gray",
        "engine": "nfa",
        "scope": "response",
        "action": "any"
    },
    "Email": {
        "loaded": true,
        "regex": "(([a-zA-Z0-9][_|\\.])*[a-zA-Z0-9]+@([a-zA-Z0-9][-|_|\\.])*[a-zA-Z0-9]+\\.((?!js|css|jpg|jpeg|png|ico)[a-zA-Z]{2,}))",
        "color": "yellow",
        "engine": "nfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: 360企业版": {
        "loaded": true,
        "regex": "(360EntInst)",
        "color": "gray",
        "engine": "dfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: 用友致远oa": {
        "loaded": true,
        "regex": "(/seeyon/USER-DATA/IMAGES/LOGIN/login.gif)",
        "color": "gray",
        "engine": "dfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: H3C公司产品": {
        "loaded": true,
        "regex": "(service@h3c.com)",
        "color": "gray",
        "engine": "dfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: H3C ICG 1000": {
        "loaded": true,
        "regex": "(ICG 1000系统管理)",
        "color": "gray",
        "engine": "nfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: Citrix-Metaframe": {
        "loaded": true,
        "regex": "(window.location=\"/Citrix/MetaFrame)",
        "color": "gray",
        "engine": "dfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: H3C ER5100": {
        "loaded": true,
        "regex": "(ER5100系统管理)",
        "color": "gray",
        "engine": "nfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: 阿里云CDN": {
        "loaded": true,
        "regex": "(cdn.aliyuncs.com)",
        "color": "gray",
        "engine": "dfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: CISCO_EPC3925": {
        "loaded": true,
        "regex": "(Docsis_system)",
        "color": "gray",
        "engine": "dfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: CISCO ASR": {
        "loaded": true,
        "regex": "(CISCO ASR)",
        "color": "gray",
        "engine": "nfa",
        "scope": "response",
        "action": "any"
    },
    "Amazon Web Services(AWS)": {
        "loaded": true,
        "regex": "((AKIA[0-9A-Z]{16})|(s3\\.amazonaws.com[/]+|[a-zA-Z0-9_-]*\\.s3\\.amazonaws.com))",
        "color": "green",
        "engine": "dfa",
        "scope": "any",
        "action": "any"
    },
    "Fingerprint: H3C ER3200": {
        "loaded": false,
        "regex": "(ER3200系统管理)",
        "color": "gray",
        "engine": "nfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: 万户ezOFFICE": {
        "loaded": true,
        "regex": "(LocLan)",
        "color": "gray",
        "engine": "dfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: 万户网络": {
        "loaded": true,
        "regex": "(css/css_whir.css)",
        "color": "gray",
        "engine": "dfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: Spark_Master": {
        "loaded": true,
        "regex": "(Spark Master at)",
        "color": "gray",
        "engine": "nfa",
        "scope": "response",
        "action": "any"
    },
    "Shiro": {
        "loaded": true,
        "regex": "(=deleteMe|rememberMe=)",
        "color": "green",
        "engine": "dfa",
        "scope": "any",
        "action": "any"
    },
    "Fingerprint: 华为_HUAWEI_SRG2220": {
        "loaded": true,
        "regex": "(HUAWEI SRG2220)",
        "color": "gray",
        "engine": "nfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: 蓝凌EIS智慧协同平台": {
        "loaded": true,
        "regex": "(/scripts/jquery.landray.common.js)",
        "color": "gray",
        "engine": "dfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: 深信服ssl-vpn": {
        "loaded": true,
        "regex": "(login_psw.csp)",
        "color": "gray",
        "engine": "dfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: 华为 NetOpen": {
        "loaded": true,
        "regex": "(/netopen/theme/css/inFrame.css)",
        "color": "gray",
        "engine": "dfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: Citrix-Web-PN-Server": {
        "loaded": true,
        "regex": "(Citrix Web PN Server)",
        "color": "gray",
        "engine": "nfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: juniper_vpn": {
        "loaded": true,
        "regex": "(welcome.cgi?p=logo)",
        "color": "gray",
        "engine": "dfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: 360主机卫士": {
        "loaded": true,
        "regex": "(X-Safe-Firewall)",
        "color": "gray",
        "engine": "dfa",
        "scope": "response",
        "action": "any"
    },
    "Alibaba OSS": {
        "loaded": true,
        "regex": "([A|a]ccess[K|k]ey[I|i][d|D]|[A|a]ccess[K|k]ey[S|s]ecret)",
        "color": "green",
        "engine": "dfa",
        "scope": "any",
        "action": "any"
    },
    "Linkfinder": {
        "loaded": false,
        "regex": "(?:\"|')(((?:[a-zA-Z]{1,10}://|//)[^\"'/]{1,}\\.[a-zA-Z]{2,}[^\"']{0,})|((?:/|\\.\\./|\\./)[^\"'><,;|*()(%%$^/\\\\\\[\\]][^\"'><,;|()]{1,})|([a-zA-Z0-9_\\-/]{1,}/[a-zA-Z0-9_\\-/]{1,}\\.(?:[a-zA-Z]{1,4}|action)(?:[\\?|#][^\"|']{0,}|))|([a-zA-Z0-9_\\-/]{1,}/[a-zA-Z0-9_\\-/]{3,}(?:[\\?|#][^\"|']{0,}|))|([a-zA-Z0-9_\\-]{1,}\\.(?:php|asp|aspx|jsp|json|action|html|js|txt|xml|do|jspx|htm)(?:[\\?|#][^\"|']{0,}|)))(?:\"|')",
        "color": "gray",
        "engine": "nfa",
        "scope": "response",
        "action": "any"
    },
    "Windows Path": {
        "loaded": true,
        "regex": "([a-zA-Z]:[\\\\/](?:[a-zA-Z0-9\\.\\-_ ]+[\\\\/])*([a-zA-Z0-9\\.\\-_ ]+))",
        "color": "green",
        "engine": "dfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: Nagios": {
        "loaded": true,
        "regex": "(Nagios access)",
        "color": "gray",
        "engine": "nfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: H3C ER8300": {
        "loaded": true,
        "regex": "(ER8300系统管理)",
        "color": "gray",
        "engine": "nfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: Citrix-Access-Gateway": {
        "loaded": true,
        "regex": "(Citrix Access Gateway)",
        "color": "gray",
        "engine": "nfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: 华为 MCU": {
        "loaded": true,
        "regex": "(McuR5-min.js)",
        "color": "gray",
        "engine": "dfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: TP-LINK Wireless WDR3600": {
        "loaded": true,
        "regex": "(TP-LINK Wireless WDR3600)",
        "color": "gray",
        "engine": "nfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: 泛微协同办公OA": {
        "loaded": true,
        "regex": "(testBanCookie)",
        "color": "gray",
        "engine": "dfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: 华为_HUAWEI_ASG2050": {
        "loaded": true,
        "regex": "(HUAWEI ASG2050)",
        "color": "gray",
        "engine": "nfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: 360网站卫士": {
        "loaded": true,
        "regex": "(360wzb)",
        "color": "gray",
        "engine": "dfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: Citrix-XenServer": {
        "loaded": true,
        "regex": "(Citrix Systems, Inc. XenServer)",
        "color": "gray",
        "engine": "nfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: H3C ER2100V2": {
        "loaded": false,
        "regex": "(ER2100V2系统管理)",
        "color": "gray",
        "engine": "nfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: zabbix": {
        "loaded": true,
        "regex": "(images/general/zabbix.ico)",
        "color": "gray",
        "engine": "dfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: CISCO_VPN": {
        "loaded": true,
        "regex": "(webvpn)",
        "color": "gray",
        "engine": "dfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: 360站长平台": {
        "loaded": true,
        "regex": "(360-site-verification)",
        "color": "gray",
        "engine": "dfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: H3C ER3108GW": {
        "loaded": true,
        "regex": "(ER3108GW系统管理)",
        "color": "gray",
        "engine": "nfa",
        "scope": "response",
        "action": "any"
    },
    "Response Password": {
        "loaded": true,
        "regex": "(\"password\":)",
        "color": "red",
        "engine": "nfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: o2security_vpn": {
        "loaded": true,
        "regex": "(client_param=install_active)",
        "color": "gray",
        "engine": "dfa",
        "scope": "response",
        "action": "any"
    },
    "JSON Web Token": {
        "loaded": true,
        "regex": "(ey[A-Za-z0-9_-]{10,}\\.[A-Za-z0-9._-]{10,}|ey[A-Za-z0-9_\\/+-]{10,}\\.[A-Za-z0-9._\\/+-]{10,})",
        "color": "green",
        "engine": "dfa",
        "scope": "any",
        "action": "any"
    },
    "Fingerprint: H3C ER3260G2": {
        "loaded": true,
        "regex": "(ER3260G2系统管理)",
        "color": "gray",
        "engine": "nfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: H3C ICG1000": {
        "loaded": true,
        "regex": "(ICG1000系统管理)",
        "color": "gray",
        "engine": "nfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: CISCO-CX20": {
        "loaded": true,
        "regex": "(CISCO-CX20)",
        "color": "gray",
        "engine": "dfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: H3C ER5200": {
        "loaded": true,
        "regex": "(ER5200系统管理)",
        "color": "gray",
        "engine": "nfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: linksys-vpn-bragap14-parintins": {
        "loaded": true,
        "regex": "(linksys-vpn-bragap14-parintins)",
        "color": "gray",
        "engine": "dfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: 360网站卫士常用前端公共库": {
        "loaded": true,
        "regex": "(libs.useso.com)",
        "color": "gray",
        "engine": "dfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: H3C ER3100": {
        "loaded": true,
        "regex": "(ER3100系统管理)",
        "color": "gray",
        "engine": "nfa",
        "scope": "response",
        "action": "any"
    },
    "Chinese IDCard": {
        "loaded": true,
        "regex": "[^0-9]((\\d{8}(0\\d|10|11|12)([0-2]\\d|30|31)\\d{3}$)|(\\d{6}(18|19|20)\\d{2}(0[1-9]|10|11|12)([0-2]\\d|30|31)\\d{3}(\\d|X|x)))[^0-9]",
        "color": "orange",
        "engine": "nfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: H3C-SecBlade-FireWall": {
        "loaded": true,
        "regex": "(js/MulPlatAPI.js)",
        "color": "gray",
        "engine": "dfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: 360webfacil_360WebManager": {
        "loaded": true,
        "regex": "(publico/template/)",
        "color": "gray",
        "engine": "dfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: Citrix_Netscaler": {
        "loaded": true,
        "regex": "(ns_af)",
        "color": "gray",
        "engine": "dfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: H3C ER6300G2": {
        "loaded": true,
        "regex": "(ER6300G2系统管理)",
        "color": "gray",
        "engine": "nfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: H3C ER3260": {
        "loaded": true,
        "regex": "(ER3260系统管理)",
        "color": "gray",
        "engine": "nfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: 华为_HUAWEI_SRG3250": {
        "loaded": true,
        "regex": "(HUAWEI SRG3250)",
        "color": "gray",
        "engine": "nfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: exchange": {
        "loaded": true,
        "regex": "(owa)",
        "color": "gray",
        "engine": "dfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: Spark_Worker": {
        "loaded": true,
        "regex": "(Spark Worker at)",
        "color": "gray",
        "engine": "nfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: H3C ER3108G": {
        "loaded": true,
        "regex": "(ER3108G系统管理)",
        "color": "gray",
        "engine": "nfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: 深信服防火墙类产品": {
        "loaded": true,
        "regex": "(SANGFOR FW)",
        "color": "gray",
        "engine": "nfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: Citrix-ConfProxy": {
        "loaded": true,
        "regex": "(confproxy)",
        "color": "gray",
        "engine": "dfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: 360网站安全检测": {
        "loaded": true,
        "regex": "(webscan.360.cn/status/pai/hash)",
        "color": "gray",
        "engine": "dfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: H3C ER5200G2": {
        "loaded": true,
        "regex": "(ER5200G2系统管理)",
        "color": "gray",
        "engine": "nfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: 华为（HUAWEI）安全设备": {
        "loaded": true,
        "regex": "(sweb-lib/resource/)",
        "color": "gray",
        "engine": "dfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: H3C ER6300": {
        "loaded": true,
        "regex": "(ER6300系统管理)",
        "color": "gray",
        "engine": "nfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: 华为_HUAWEI_ASG2100": {
        "loaded": true,
        "regex": "(HUAWEI ASG2100)",
        "color": "gray",
        "engine": "nfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: TP-Link 3600 DD-WRT": {
        "loaded": true,
        "regex": "(TP-Link 3600 DD-WRT)",
        "color": "gray",
        "engine": "nfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: NETGEAR WNDR3600": {
        "loaded": true,
        "regex": "(NETGEAR WNDR3600)",
        "color": "gray",
        "engine": "nfa",
        "scope": "response",
        "action": "any"
    },
    "Chinese Mobile Number": {
        "loaded": true,
        "regex": "[^0-9](1(3([0-35-9]\\d|4[1-8])|4[14-9]\\d|5([\\d]\\d|7[1-79])|66\\d|7[2-35-8]\\d|8\\d{2}|9[89]\\d)\\d{7})[^0-9]",
        "color": "orange",
        "engine": "nfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: H3C ER2100": {
        "loaded": true,
        "regex": "(ER2100系统管理)",
        "color": "gray",
        "engine": "nfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: 绿盟下一代防火墙": {
        "loaded": true,
        "regex": "(NSFOCUS NF)",
        "color": "gray",
        "engine": "nfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: jira": {
        "loaded": true,
        "regex": "(jira.webresources)",
        "color": "gray",
        "engine": "dfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: 金和协同管理平台": {
        "loaded": true,
        "regex": "(金和协同管理平台)",
        "color": "gray",
        "engine": "nfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: Citrix-NetScaler": {
        "loaded": true,
        "regex": "(NS-CACHE)",
        "color": "gray",
        "engine": "dfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: linksys-vpn": {
        "loaded": true,
        "regex": "(linksys-vpn)",
        "color": "gray",
        "engine": "dfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: 通达OA": {
        "loaded": true,
        "regex": "(<link rel=\"shortcut icon\" href=\"/images/tongda.ico\" />)",
        "color": "gray",
        "engine": "nfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: 华为（HUAWEI）Secoway设备": {
        "loaded": true,
        "regex": "(Secoway)",
        "color": "gray",
        "engine": "dfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: 华为_HUAWEI_SRG1220": {
        "loaded": true,
        "regex": "(HUAWEI SRG1220)",
        "color": "gray",
        "engine": "nfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: H3C ER2100n": {
        "loaded": true,
        "regex": "(ER2100n系统管理)",
        "color": "gray",
        "engine": "nfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: H3C ER8300G2": {
        "loaded": true,
        "regex": "(ER8300G2系统管理)",
        "color": "gray",
        "engine": "nfa",
        "scope": "response",
        "action": "any"
    },
    "Fingerprint: 金蝶政务GSiS": {
        "loaded": true,
        "regex": "(/kdgs/script/kdgs.js)",
        "color": "gray",
        "engine": "dfa",
        "scope": "response",
        "action": "any"
    }
}
```