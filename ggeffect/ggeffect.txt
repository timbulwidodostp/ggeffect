# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Get marginal effects from model terms Use ggeffect (ggeffects) With (In) R Software
install.packages("ggeffects")
install.packages("effects")
install.packages("nloptr")
install.packages("reformulas")
install.packages("ggplot2")
library("ggeffects")
ggeffect = read.csv("https://raw.githubusercontent.com/timbulwidodostp/ggeffect/main/ggeffect/ggeffect.csv",sep = ";")
# Estimation Get marginal effects from model terms Use ggeffect (ggeffects) With (In) R Software
ggeffect_lm <- lm(ggeffect ~ ggeffect_1 + ggeffect_2 + ggeffect_3, data = ggeffect)
ggeffect <- ggeffect(ggeffect_lm, terms = c("ggeffect_1", "ggeffect_2", "ggeffect_3"))
ggeffect
plot(ggeffect)
# Get marginal effects from model terms Use ggeffect (ggeffects) With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished
