# ****************************************************************************
# @@@ START COPYRIGHT @@@
#
# (C) Copyright 2007-2014 Hewlett-Packard Development Company, L.P.
#
#  Licensed under the Apache License, Version 2.0 (the "License");
#  you may not use this file except in compliance with the License.
#  You may obtain a copy of the License at
#
#      http://www.apache.org/licenses/LICENSE-2.0
#
#  Unless required by applicable law or agreed to in writing, software
#  distributed under the License is distributed on an "AS IS" BASIS,
#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
#  See the License for the specific language governing permissions and
#  limitations under the License.
#
# @@@ END COPYRIGHT @@@
# ****************************************************************************

ifeq (,$(filter $(TARGTYPE),oss yos))
  %(error The report library can be built only for NSK platforms)
endif

CPPSRC := RWUtils.cpp\
	RWTracer.cpp\
	RWTotalList.cpp\
	RWTitleFooting.cpp\
	RWTabClass.cpp\
	RWSubtotalList.cpp\
	RWstyle.cpp\
	RWStringLiteral.cpp\
	RWSpaceClass.cpp\
	RWSkipClass.cpp\
	RWSelectList.cpp\
	RWReportDefinition.cpp\
	RWPrintableDetailItem.cpp\
	RWPageClass.cpp\
	RWOutputBuffer.cpp\
	RWNumericExpression.cpp\
	RWNonPrintableDetailItem.cpp\
	RWNestedList.cpp\
	RWNeedClass.cpp\
	RWLayout.cpp\
	RWInputBuffer.cpp\
	RWIfThenElse.cpp\
	RWHeading.cpp\
	RWFormatItemList.cpp\
	RWFormatItem.cpp\
	RWFormatDecimal.cpp\
	RWFormatBuffer.cpp\
	RWFormat.cpp\
	RWErrorSet.cpp\
	RWEnv.cpp\
	RWDTExpressionNode.cpp\
	RWDTExpression.cpp\
	RWDetailList.cpp\
	RWDetailItem.cpp\
	RWDetail.cpp\
	RWConditionalExpressionNode.cpp\
	RWConcat.cpp\
	RWColumnValue.cpp\
	RWColumnId.cpp\
	RWBreakItem.cpp\
	RWBreakGroup.cpp\
	RWAliasList.cpp\
	RWParsedQueryList.cpp\
	RWInterface.cpp

YSRC := rep_yacc.y
LSRC := rep_lex.ll
LEX_PREFIX := rw
YACC_VAR_PREFIX := rw

DEFS := -DSQLCLI_LIB

SRCPATH := report sqlci

$(TARGOBJDIR)/$(LEX_PREFIX)rep_lex.$(OBJSUFFIX): $(TARGOBJDIR)/rep_yacc.h
