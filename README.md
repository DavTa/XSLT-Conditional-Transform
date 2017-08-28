# XSLT-Conditional-Transform

<xsl:if test= "normalize-space(RelatedBenefitLimitStatuses/ClaimedAmount) != ''">
	<xsl:element name="ClaimedAmount" xmlns = "http://schemas.hambs.com.au/external/membership/getmembershipbenefitlimitstatuses/membershipperson/2014/06">
		<xsl:value-of select="/root:GetMembershipBenefitLimitStatusesResponse/MembershipPersons/SpecialityClasses/SpecialityClass/BenefitLimitStatuses/BenefitLimitStatus/RelatedBenefitLimitStatuses/ClaimedAmount" />
	</xsl:element>
</xsl:if>
