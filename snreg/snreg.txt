# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Linear Regression with Skew-Normal Errors Use snreg With (In) R Software
install.packages("snreg")
library("snreg")
# Estimation Linear Regression with Skew-Normal Errors Use snreg With (In) R Software
snreg = read.csv("https://raw.githubusercontent.com/timbulwidodostp/snreg/main/snreg/snreg.csv",sep = ";")
spe.tl <- log(TC) ~ (log(Y1) + log(Y2) + log(W1) + log(W2))^2 + I(0.5 * log(Y1)^2) + I(0.5 * log(Y2)^2) + I(0.5 * log(W1)^2) + I(0.5 * log(W2)^2)
formSV <- NULL
formSK <- NULL
snreg <- snreg(formula = spe.tl, data = snreg, ln.var.v = formSV, skew.v = formSK)
summary(snreg)
# Linear Regression with Skew-Normal Errors Use snreg With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished