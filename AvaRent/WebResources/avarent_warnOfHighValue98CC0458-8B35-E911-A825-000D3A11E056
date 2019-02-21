function showWarning(executionContext) {
	var formContext = executionContext.getFormContext();  
	if (Xrm.Page.getAttribute("avarent_highvalue").getValue()) {
		formContext.ui.setFormNotification("High Value Tenant", "WARNING", "highValueWarning");  
	} else {
		formContext.ui.clearFormNotification("highValueWarning");  
	}
}

function appendStyle() {
	parent.$("head").append("<style>#crmNotifications { background-color: purple; } #Notification0_text { color: white !important; }</style>");
}

function setIframe() {
	var value = Xrm.Page.getAttribute("websiteurl").getValue();
	if (value) {
		Xrm.Page.getControl("IFRAME_tenantwebsite").setSrc(value);		
	}
}
