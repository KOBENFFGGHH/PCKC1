--[[
This script is protected by XProtect Obfuscator Free Version.

Version: 1.0
Obfuscation Time: 582ms

For support and updates, join our Discord community:
Discord: discord.gg/7hv7k6FfNr

]]
local f=string.byte;local r=string.char;local c=string.sub;local s=table.concat;local G=math.ldexp;local B=getfenv or function()return _ENV end;local l=setmetatable;local u=select;local i=unpack;local h=tonumber;local function b(t)local e,o,n="","",{}local d=256;local a={}for l=0,d-1 do a[l]=r(l)end;local l=1;local function f()local e=h(c(t,l,l),36)l=l+1;local o=h(c(t,l,l+e-1),36)l=l+e;return o end;e=r(f())n[1]=e;while l<#t do local l=f()if a[l]then o=a[l]else o=e..c(e,1,1)end;a[d]=e..c(o,1,1)n[#n+1],e,d=o,o,d+1 end;return table.concat(n)end;local a=b('22922G27525622824O24N22W22827525A22027923C22027525B22822W22G23C27C22G25223C27G23C27524R27P27O27J27U27N28025727N28427525722827I27Y22G28727528A22K27522G22J22A28G21G21J21L21O21721821621D21I21R22J28F27521R21L21H21P22J22N28G1G2182182141V21P21822J1P28G21C29621421722Q23B23B21621L21B23A21R21D21821C21921M21921721P21621N21J21I21821P2A223A2A021H23B1J1N1Q1T1M1U1U1V1V1G1G23B181R2AA23B21H21L28S23B1A1T1P1S1L1T23A21H21O28G275');local n=bit and bit.bxor or function(l,o)local e,n=1,0 while l>0 and o>0 do local a,c=l%2,o%2 if a~=c then n=n+e end l,o,e=(l-a)/2,(o-c)/2,e*2 end if l<o then l=o end while l>0 do local o=l%2 if o>0 then n=n+e end l,e=(l-o)/2,e*2 end return n end local function e(o,l,e)if e then local l=(o/2^(l-1))%2^((e-1)-(l-1)+1);return l-l%1;else local l=2^(l-1);return(o%(l+l)>=l)and 1 or 0;end;end;local l=1;local function o()local o,e,c,a=f(a,l,l+3);o=n(o,88)e=n(e,88)c=n(c,88)a=n(a,88)l=l+4;return(a*16777216)+(c*65536)+(e*256)+o;end;local function d()local e=n(f(a,l,l),88);l=l+1;return e;end;local function h()local l=o();local n=o();local c=1;local o=(e(n,1,20)*(2^32))+l;local l=e(n,21,31);local e=((-1)^e(n,32));if(l==0)then if(o==0)then return e*0;else l=1;c=0;end;elseif(l==2047)then return(o==0)and(e*(1/0))or(e*(0/0));end;return G(e,l-1023)*(c+(o/(2^52)));end;local t=o;local function G(e)local o;if(not e)then e=t();if(e==0)then return'';end;end;o=c(a,l,l+e-1);l=l+e;local e={}for l=1,#o do e[l]=r(n(f(c(o,l,l)),88))end return s(e);end;local l=o;local function f(...)return{...},u('#',...)end local function b()local t={0,0,0,0,0,0,0,0,0};local r={};local l={};local a={t,nil,r,nil,l};for a=1,o()do local c=n(o(),227);local o=n(o(),32);local n=e(c,1,2);local l=e(o,1,11);local l={l,e(c,3,11),nil,nil,o};if(n==0)then l[3]=e(c,12,20);l[5]=e(c,21,29);elseif(n==1)then l[3]=e(o,12,33);elseif(n==2)then l[3]=e(o,12,32)-1048575;elseif(n==3)then l[3]=e(o,12,32)-1048575;l[5]=e(c,21,29);end;t[a]=l;end;local l=o()local n={0,0,0,0};for o=1,l do local e=d();local l;if(e==1)then l=(d()~=0);elseif(e==0)then l=h();elseif(e==3)then l=G();end;n[o]=l;end;a[2]=n a[4]=d();for l=1,o()do r[l-1]=b();end;return a;end;local function J(l,e,h)local n=l[1];local o=l[2];local e=l[3];local l=l[4];return function(...)local r=n;local t=o;local e=e;local n=l;local s=f local o=1;local d=-1;local f={};local c={...};local a=u('#',...)-1;local l={};local e={};for l=0,a do if(l>=n)then f[l-n]=c[l+1];else e[l]=c[l+1];end;end;local l=a-n+1 local l;local n;while true do l=r[o];n=l[1];if n<=7 then if n<=3 then if n<=1 then if n==0 then local n=l[2];local o=e[l[3]];e[n+1]=o;e[n]=o[t[l[5]]];else do return end;end;elseif n>2 then e[l[2]]=t[l[3]];else e[l[2]]=h[t[l[3]]];end;elseif n<=5 then if n>4 then e[l[2]]();d=A;else local n=l[2];local c={};local o=0;local a=d;for l=n+1,a do o=o+1;c[o]=e[l];end;local c={e[n](i(c,1,a-n))};local l=n+l[5]-2;o=0;for l=n,l do o=o+1;e[l]=c[o];end;d=l;end;elseif n==6 then e[l[2]]();d=A;else e[l[2]]=(l[3]~=0);end;elseif n<=11 then if n<=9 then if n==8 then local n=l[2];local c={};local o=0;local l=n+l[3]-1;for l=n+1,l do o=o+1;c[o]=e[l];end;local c,l=s(e[n](i(c,1,l-n)));l=l+n-1;o=0;for l=n,l do o=o+1;e[l]=c[o];end;d=l;else e[l[2]]=(l[3]~=0);end;elseif n>10 then do return end;else e[l[2]]=t[l[3]];end;elseif n<=13 then if n>12 then local n=l[2];local a={};local o=0;local c=d;for l=n+1,c do o=o+1;a[o]=e[l];end;local c={e[n](i(a,1,c-n))};local l=n+l[5]-2;o=0;for l=n,l do o=o+1;e[l]=c[o];end;d=l;else e[l[2]]=h[t[l[3]]];end;elseif n<=14 then local n=l[2];local c={};local o=0;local l=n+l[3]-1;for l=n+1,l do o=o+1;c[o]=e[l];end;local c,l=s(e[n](i(c,1,l-n)));l=l+n-1;o=0;for l=n,l do o=o+1;e[l]=c[o];end;d=l;elseif n>15 then local n;local u,n;local a;local c;local f;local G;local n;e[l[2]]=h[t[l[3]]];o=o+1;l=r[o];e[l[2]]=h[t[l[3]]];o=o+1;l=r[o];n=l[2];G=e[l[3]];e[n+1]=G;e[n]=G[t[l[5]]];o=o+1;l=r[o];e[l[2]]=t[l[3]];o=o+1;l=r[o];e[l[2]]=(l[3]~=0);o=o+1;l=r[o];n=l[2];f={};c=0;a=n+l[3]-1;for l=n+1,a do c=c+1;f[c]=e[l];end;u,a=s(e[n](i(f,1,a-n)));a=a+n-1;c=0;for l=n,a do c=c+1;e[l]=u[c];end;d=a;o=o+1;l=r[o];n=l[2];f={};c=0;a=d;for l=n+1,a do c=c+1;f[c]=e[l];end;u={e[n](i(f,1,a-n))};a=n+l[5]-2;c=0;for l=n,a do c=c+1;e[l]=u[c];end;d=a;o=o+1;l=r[o];e[l[2]]();d=n;o=o+1;l=r[o];do return end;else local n=l[2];local o=e[l[3]];e[n+1]=o;e[n]=o[t[l[5]]];end;o=o+1;end;end;end;return J(b(),{},B())();
