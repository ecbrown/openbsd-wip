# $OpenBSD: Makefile,v 1.9 2018/06/04 20:25:32 rsadowski Exp $

COMMENT =	integration of QML and KDE workspaces
DISTNAME =	kdeclarative-${VERSION}

SHARED_LIBS =	KF5Declarative		4.2 # 5.17
SHARED_LIBS +=	KF5CalendarEvents	4.2 # 5.17
SHARED_LIBS +=	KF5QuickAddons		4.2 # 5.17

WANTLIB += ${COMPILER_LIBCXX} KF5Completion KF5ConfigCore KF5ConfigGui
WANTLIB += KF5CoreAddons KF5GlobalAccel KF5I18n KF5IconThemes
WANTLIB += KF5JobWidgets KF5KIOCore KF5KIOWidgets KF5Package KF5Service
WANTLIB += KF5WidgetsAddons KF5WindowSystem Qt5Concurrent Qt5Core
WANTLIB += Qt5DBus Qt5Gui Qt5Network Qt5Qml Qt5Quick Qt5Widgets
WANTLIB += Qt5Xml c epoxy m

BUILD_DEPENDS =	devel/gettext-tools \
		devel/kf5/kguiaddons

RUN_DEPENDS =	devel/kf5/kguiaddons

LIB_DEPENDS =	devel/kf5/kconfig \
		devel/kf5/kglobalaccel \
		devel/kf5/ki18n \
		devel/kf5/kiconthemes \
		devel/kf5/kio \
		devel/kf5/kpackage \
		devel/kf5/kwidgetsaddons \
		devel/kf5/kwindowsystem \
		x11/qt5/qtdeclarative

TEST_IS_INTERACTIVE =	X11
PORTHOME =		${WRKDIR}

.include <bsd.port.mk>
