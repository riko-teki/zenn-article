---
title: "CpawCTF level1 Classical Cipher Writeup"
emoji: "ð»"
type: "tech"
topics: ["ctf","crypto"]
published: true
---

# åé¡
æå·ã«ã¯å¤§ããåãã¦ãå¤å¸æå·ã¨ç¾ä»£æå·ã®2ç¨®é¡ãããã¾ãã  
ç¹ã«å¤å¸æå·ã§ã¯ãå¤ä»£ã­ã¼ãã®è»äºçæå°èã¬ã¤ã¦ã¹ã»ã¦ãªã¦ã¹ã»ã«ã¨ãµã«ï¼è±èªèª­ã¿ã§ã·ã¼ã¶ã¼ï¼ãåãã¦ä½¿ã£ããã¨ãããåç§°ãã¤ããã·ã¼ã¶ã¼æå·ãæåã§ãã  
ããã¯3æå­åã¢ã«ãã¡ãããããããã¨ããåä¸æå­å¼æå·ã®ä¸ã¤ã§ãã  
æ¬¡ã®æå·æã¯ããã®ã·ã¼ã¶ã¼æå·ãç¨ãã¦æå·åãã¾ãããæå·æãè§£èª­ãã¦ãã©ã°ãæã«ããã¾ãããã

æå·æ: fsdz{Fdhvdu_flskhu_lv_fodvvlfdo_flskhu}

# Flagã®å¥ææ¹æ³
åé¡æã«æ¸ãã¦ããéãã§ãã
åæå­ã3æå­ãããã¦ããã°Flagãæã«å¥ãã¾ãã
D â A
E â B

# ã½ã«ã

```julia
c = "fsdz{Fdhvdu_flskhu_lv_fodvvlfdo_flskhu}"

for s in c
  if (Int(s) >= 65 && Int(s) <= 90) || (Int(s) >= 97 && Int(s) <= 122)
    print(Char(Int(s)-3))
  else
    print(s)
  end
end

```