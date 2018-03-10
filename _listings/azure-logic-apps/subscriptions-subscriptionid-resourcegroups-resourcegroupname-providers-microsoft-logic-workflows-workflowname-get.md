---
swagger: "2.0"
info:
  title: LogicManagementClient
  description: REST API for Azure Logic Apps.
  version: 1.0.0
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/workflows/{workflowName}:
    get:
      summary: Workflows Get
      description: Gets a workflow
      operationId: Workflows_Get
      parameters:
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The resource group name
      - in: path
        name: workflowName
        description: The workflow name
      responses:
        200:
          description: OK
      tags:
      - workflows
definitions:
  Resource:
    properties:
      id:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      type:
        description: This is a default description.
        type: get
      location:
        description: This is a default description.
        type: get
      tags:
        description: This is a default description.
        type: get
  SubResource:
    properties:
      id:
        description: This is a default description.
        type: get
  Object:
    properties: []
  ResourceReference:
    properties:
      id:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      type:
        description: This is a default description.
        type: get
  Workflow:
    properties: []
  WorkflowProperties:
    properties:
      createdTime:
        description: This is a default description.
        type: get
      changedTime:
        description: This is a default description.
        type: get
      version:
        description: This is a default description.
        type: get
      accessEndpoint:
        description: This is a default description.
        type: get
      parameters:
        description: This is a default description.
        type: get
  WorkflowFilter:
    properties: []
  WorkflowListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  WorkflowVersion:
    properties: []
  WorkflowVersionProperties:
    properties:
      createdTime:
        description: This is a default description.
        type: get
      changedTime:
        description: This is a default description.
        type: get
      version:
        description: This is a default description.
        type: get
      accessEndpoint:
        description: This is a default description.
        type: get
      parameters:
        description: This is a default description.
        type: get
  WorkflowVersionListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  WorkflowTrigger:
    properties:
      name:
        description: This is a default description.
        type: get
      type:
        description: This is a default description.
        type: get
  WorkflowTriggerProperties:
    properties:
      createdTime:
        description: This is a default description.
        type: get
      changedTime:
        description: This is a default description.
        type: get
      lastExecutionTime:
        description: This is a default description.
        type: get
      nextExecutionTime:
        description: This is a default description.
        type: get
  WorkflowTriggerFilter:
    properties: []
  WorkflowTriggerListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  WorkflowTriggerCallbackUrl:
    properties:
      value:
        description: This is a default description.
        type: get
      method:
        description: This is a default description.
        type: get
      basePath:
        description: This is a default description.
        type: get
      relativePath:
        description: This is a default description.
        type: get
      relativePathParameters:
        description: This is a default description.
        type: get
  WorkflowTriggerListCallbackUrlQueries:
    properties:
      api-version:
        description: This is a default description.
        type: get
      sp:
        description: This is a default description.
        type: get
      sv:
        description: This is a default description.
        type: get
      sig:
        description: This is a default description.
        type: get
  WorkflowTriggerHistory:
    properties:
      name:
        description: This is a default description.
        type: get
      type:
        description: This is a default description.
        type: get
  WorkflowTriggerHistoryProperties:
    properties:
      startTime:
        description: This is a default description.
        type: get
      endTime:
        description: This is a default description.
        type: get
      code:
        description: This is a default description.
        type: get
      trackingId:
        description: This is a default description.
        type: get
      fired:
        description: This is a default description.
        type: get
  WorkflowTriggerHistoryListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  WorkflowTriggerHistoryFilter:
    properties: []
  WorkflowRun:
    properties:
      name:
        description: This is a default description.
        type: get
      type:
        description: This is a default description.
        type: get
  WorkflowRunProperties:
    properties:
      startTime:
        description: This is a default description.
        type: get
      endTime:
        description: This is a default description.
        type: get
      code:
        description: This is a default description.
        type: get
      correlationId:
        description: This is a default description.
        type: get
      outputs:
        description: This is a default description.
        type: get
  WorkflowRunFilter:
    properties: []
  WorkflowRunListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  WorkflowRunAction:
    properties:
      name:
        description: This is a default description.
        type: get
      type:
        description: This is a default description.
        type: get
  WorkflowRunActionProperties:
    properties:
      startTime:
        description: This is a default description.
        type: get
      endTime:
        description: This is a default description.
        type: get
      code:
        description: This is a default description.
        type: get
      trackingId:
        description: This is a default description.
        type: get
      retryHistory:
        description: This is a default description.
        type: get
  WorkflowRunActionFilter:
    properties: []
  WorkflowRunActionListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  Sku:
    properties: []
  ContentLink:
    properties:
      uri:
        description: This is a default description.
        type: get
      contentVersion:
        description: This is a default description.
        type: get
      contentSize:
        description: This is a default description.
        type: get
  ContentHash:
    properties:
      algorithm:
        description: This is a default description.
        type: get
      value:
        description: This is a default description.
        type: get
  RegenerateActionParameter:
    properties: []
  RetryHistory:
    properties:
      startTime:
        description: This is a default description.
        type: get
      endTime:
        description: This is a default description.
        type: get
      code:
        description: This is a default description.
        type: get
      clientRequestId:
        description: This is a default description.
        type: get
      serviceRequestId:
        description: This is a default description.
        type: get
  Correlation:
    properties:
      clientTrackingId:
        description: This is a default description.
        type: get
  WorkflowParameter:
    properties:
      description:
        description: This is a default description.
        type: get
  WorkflowOutputParameter:
    properties: []
  RecurrenceSchedule:
    properties:
      minutes:
        description: This is a default description.
        type: get
      hours:
        description: This is a default description.
        type: get
      weekDays:
        description: This is a default description.
        type: get
      monthDays:
        description: This is a default description.
        type: get
      monthlyOccurrences:
        description: This is a default description.
        type: get
  RecurrenceScheduleOccurrence:
    properties:
      occurrence:
        description: This is a default description.
        type: get
  WorkflowTriggerRecurrence:
    properties:
      interval:
        description: This is a default description.
        type: get
      startTime:
        description: This is a default description.
        type: get
      endTime:
        description: This is a default description.
        type: get
      timeZone:
        description: This is a default description.
        type: get
  WorkflowRunTrigger:
    properties:
      name:
        description: This is a default description.
        type: get
      startTime:
        description: This is a default description.
        type: get
      endTime:
        description: This is a default description.
        type: get
      trackingId:
        description: This is a default description.
        type: get
      code:
        description: This is a default description.
        type: get
  GenerateUpgradedDefinitionParameters:
    properties:
      targetSchemaVersion:
        description: This is a default description.
        type: get
  IntegrationAccount:
    properties: []
  IntegrationAccountProperties:
    properties: []
  IntegrationAccountListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  GetCallbackUrlParameters:
    properties:
      notAfter:
        description: This is a default description.
        type: get
  CallbackUrl:
    properties:
      value:
        description: This is a default description.
        type: get
  IntegrationAccountSchema:
    properties: []
  IntegrationAccountSchemaProperties:
    properties:
      targetNamespace:
        description: This is a default description.
        type: get
      documentName:
        description: This is a default description.
        type: get
      fileName:
        description: This is a default description.
        type: get
      createdTime:
        description: This is a default description.
        type: get
      changedTime:
        description: This is a default description.
        type: get
      metadata:
        description: This is a default description.
        type: get
      content:
        description: This is a default description.
        type: get
      contentType:
        description: This is a default description.
        type: get
  IntegrationAccountSchemaListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  IntegrationAccountSchemaFilter:
    properties: []
  IntegrationAccountMap:
    properties: []
  IntegrationAccountMapProperties:
    properties:
      parametersSchema:
        description: This is a default description.
        type: get
      createdTime:
        description: This is a default description.
        type: get
      changedTime:
        description: This is a default description.
        type: get
      content:
        description: This is a default description.
        type: get
      contentType:
        description: This is a default description.
        type: get
      metadata:
        description: This is a default description.
        type: get
  IntegrationAccountMapListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  IntegrationAccountMapFilter:
    properties: []
  IntegrationAccountSku:
    properties: []
  IntegrationAccountPartnerListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  IntegrationAccountPartnerFilter:
    properties: []
  IntegrationAccountPartner:
    properties: []
  IntegrationAccountPartnerProperties:
    properties:
      createdTime:
        description: This is a default description.
        type: get
      changedTime:
        description: This is a default description.
        type: get
      metadata:
        description: This is a default description.
        type: get
  PartnerContent:
    properties: []
  B2BPartnerContent:
    properties:
      businessIdentities:
        description: This is a default description.
        type: get
  BusinessIdentity:
    properties:
      qualifier:
        description: This is a default description.
        type: get
      value:
        description: This is a default description.
        type: get
  IntegrationAccountAgreementListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  IntegrationAccountAgreementFilter:
    properties: []
  IntegrationAccountAgreement:
    properties: []
  IntegrationAccountAgreementProperties:
    properties:
      createdTime:
        description: This is a default description.
        type: get
      changedTime:
        description: This is a default description.
        type: get
      metadata:
        description: This is a default description.
        type: get
      hostPartner:
        description: This is a default description.
        type: get
      guestPartner:
        description: This is a default description.
        type: get
  AgreementContent:
    properties: []
  AS2AgreementContent:
    properties: []
  AS2OneWayAgreement:
    properties: []
  AS2ProtocolSettings:
    properties: []
  AS2AcknowledgementConnectionSettings:
    properties:
      ignoreCertificateNameMismatch:
        description: This is a default description.
        type: get
      supportHttpStatusCodeContinue:
        description: This is a default description.
        type: get
      keepHttpConnectionAlive:
        description: This is a default description.
        type: get
      unfoldHttpHeaders:
        description: This is a default description.
        type: get
  AS2MessageConnectionSettings:
    properties:
      ignoreCertificateNameMismatch:
        description: This is a default description.
        type: get
      supportHttpStatusCodeContinue:
        description: This is a default description.
        type: get
      keepHttpConnectionAlive:
        description: This is a default description.
        type: get
      unfoldHttpHeaders:
        description: This is a default description.
        type: get
  AS2MdnSettings:
    properties:
      needMdn:
        description: This is a default description.
        type: get
      signMdn:
        description: This is a default description.
        type: get
      sendMdnAsynchronously:
        description: This is a default description.
        type: get
      receiptDeliveryUrl:
        description: This is a default description.
        type: get
      dispositionNotificationTo:
        description: This is a default description.
        type: get
      signOutboundMdnIfOptional:
        description: This is a default description.
        type: get
      mdnText:
        description: This is a default description.
        type: get
      sendInboundMdnToMessageBox:
        description: This is a default description.
        type: get
  AS2SecuritySettings:
    properties:
      overrideGroupSigningCertificate:
        description: This is a default description.
        type: get
      signingCertificateName:
        description: This is a default description.
        type: get
      encryptionCertificateName:
        description: This is a default description.
        type: get
      enableNrrForInboundEncodedMessages:
        description: This is a default description.
        type: get
      enableNrrForInboundDecodedMessages:
        description: This is a default description.
        type: get
      enableNrrForOutboundMdn:
        description: This is a default description.
        type: get
      enableNrrForOutboundEncodedMessages:
        description: This is a default description.
        type: get
      enableNrrForOutboundDecodedMessages:
        description: This is a default description.
        type: get
      enableNrrForInboundMdn:
        description: This is a default description.
        type: get
      sha2AlgorithmFormat:
        description: This is a default description.
        type: get
  AS2ValidationSettings:
    properties:
      overrideMessageProperties:
        description: This is a default description.
        type: get
      encryptMessage:
        description: This is a default description.
        type: get
      signMessage:
        description: This is a default description.
        type: get
      compressMessage:
        description: This is a default description.
        type: get
      checkDuplicateMessage:
        description: This is a default description.
        type: get
      interchangeDuplicatesValidityDays:
        description: This is a default description.
        type: get
      checkCertificateRevocationListOnSend:
        description: This is a default description.
        type: get
      checkCertificateRevocationListOnReceive:
        description: This is a default description.
        type: get
  AS2EnvelopeSettings:
    properties:
      messageContentType:
        description: This is a default description.
        type: get
      transmitFileNameInMimeHeader:
        description: This is a default description.
        type: get
      fileNameTemplate:
        description: This is a default description.
        type: get
      suspendMessageOnFileNameGenerationError:
        description: This is a default description.
        type: get
      autogenerateFileName:
        description: This is a default description.
        type: get
  AS2ErrorSettings:
    properties:
      suspendDuplicateMessage:
        description: This is a default description.
        type: get
      resendIfMdnNotReceived:
        description: This is a default description.
        type: get
  X12AgreementContent:
    properties: []
  X12OneWayAgreement:
    properties: []
  X12ProtocolSettings:
    properties:
      envelopeOverrides:
        description: This is a default description.
        type: get
      validationOverrides:
        description: This is a default description.
        type: get
      messageFilterList:
        description: This is a default description.
        type: get
      schemaReferences:
        description: This is a default description.
        type: get
      x12DelimiterOverrides:
        description: This is a default description.
        type: get
  X12ValidationSettings:
    properties:
      validateCharacterSet:
        description: This is a default description.
        type: get
      checkDuplicateInterchangeControlNumber:
        description: This is a default description.
        type: get
      interchangeControlNumberValidityDays:
        description: This is a default description.
        type: get
      checkDuplicateGroupControlNumber:
        description: This is a default description.
        type: get
      checkDuplicateTransactionSetControlNumber:
        description: This is a default description.
        type: get
      validateEdiTypes:
        description: This is a default description.
        type: get
      validateXsdTypes:
        description: This is a default description.
        type: get
      allowLeadingAndTrailingSpacesAndZeroes:
        description: This is a default description.
        type: get
      trimLeadingAndTrailingSpacesAndZeroes:
        description: This is a default description.
        type: get
  X12FramingSettings:
    properties:
      dataElementSeparator:
        description: This is a default description.
        type: get
      componentSeparator:
        description: This is a default description.
        type: get
      replaceSeparatorsInPayload:
        description: This is a default description.
        type: get
      replaceCharacter:
        description: This is a default description.
        type: get
      segmentTerminator:
        description: This is a default description.
        type: get
  X12EnvelopeSettings:
    properties:
      controlStandardsId:
        description: This is a default description.
        type: get
      useControlStandardsIdAsRepetitionCharacter:
        description: This is a default description.
        type: get
      senderApplicationId:
        description: This is a default description.
        type: get
      receiverApplicationId:
        description: This is a default description.
        type: get
      controlVersionNumber:
        description: This is a default description.
        type: get
      interchangeControlNumberLowerBound:
        description: This is a default description.
        type: get
      interchangeControlNumberUpperBound:
        description: This is a default description.
        type: get
      rolloverInterchangeControlNumber:
        description: This is a default description.
        type: get
      enableDefaultGroupHeaders:
        description: This is a default description.
        type: get
      functionalGroupId:
        description: This is a default description.
        type: get
  X12AcknowledgementSettings:
    properties:
      needTechnicalAcknowledgement:
        description: This is a default description.
        type: get
      batchTechnicalAcknowledgements:
        description: This is a default description.
        type: get
      needFunctionalAcknowledgement:
        description: This is a default description.
        type: get
      functionalAcknowledgementVersion:
        description: This is a default description.
        type: get
      batchFunctionalAcknowledgements:
        description: This is a default description.
        type: get
      needImplementationAcknowledgement:
        description: This is a default description.
        type: get
      implementationAcknowledgementVersion:
        description: This is a default description.
        type: get
      batchImplementationAcknowledgements:
        description: This is a default description.
        type: get
      needLoopForValidMessages:
        description: This is a default description.
        type: get
      sendSynchronousAcknowledgement:
        description: This is a default description.
        type: get
  X12MessageFilter:
    properties: []
  X12SecuritySettings:
    properties:
      authorizationQualifier:
        description: This is a default description.
        type: get
      authorizationValue:
        description: This is a default description.
        type: get
      securityQualifier:
        description: This is a default description.
        type: get
      passwordValue:
        description: This is a default description.
        type: get
  X12ProcessingSettings:
    properties:
      maskSecurityInfo:
        description: This is a default description.
        type: get
      convertImpliedDecimal:
        description: This is a default description.
        type: get
      preserveInterchange:
        description: This is a default description.
        type: get
      suspendInterchangeOnError:
        description: This is a default description.
        type: get
      createEmptyXmlTagsForTrailingSeparators:
        description: This is a default description.
        type: get
      useDotAsDecimalSeparator:
        description: This is a default description.
        type: get
  X12EnvelopeOverride:
    properties:
      targetNamespace:
        description: This is a default description.
        type: get
      protocolVersion:
        description: This is a default description.
        type: get
      messageId:
        description: This is a default description.
        type: get
      responsibleAgencyCode:
        description: This is a default description.
        type: get
      headerVersion:
        description: This is a default description.
        type: get
      senderApplicationId:
        description: This is a default description.
        type: get
      receiverApplicationId:
        description: This is a default description.
        type: get
      functionalIdentifierCode:
        description: This is a default description.
        type: get
  X12ValidationOverride:
    properties:
      messageId:
        description: This is a default description.
        type: get
      validateEdiTypes:
        description: This is a default description.
        type: get
      validateXsdTypes:
        description: This is a default description.
        type: get
      allowLeadingAndTrailingSpacesAndZeroes:
        description: This is a default description.
        type: get
      validateCharacterSet:
        description: This is a default description.
        type: get
      trimLeadingAndTrailingSpacesAndZeroes:
        description: This is a default description.
        type: get
  X12MessageIdentifier:
    properties:
      messageId:
        description: This is a default description.
        type: get
  X12SchemaReference:
    properties:
      messageId:
        description: This is a default description.
        type: get
      senderApplicationId:
        description: This is a default description.
        type: get
      schemaVersion:
        description: This is a default description.
        type: get
      schemaName:
        description: This is a default description.
        type: get
  X12DelimiterOverrides:
    properties:
      protocolVersion:
        description: This is a default description.
        type: get
      messageId:
        description: This is a default description.
        type: get
      dataElementSeparator:
        description: This is a default description.
        type: get
      componentSeparator:
        description: This is a default description.
        type: get
      segmentTerminator:
        description: This is a default description.
        type: get
      replaceCharacter:
        description: This is a default description.
        type: get
      replaceSeparatorsInPayload:
        description: This is a default description.
        type: get
      targetNamespace:
        description: This is a default description.
        type: get
  EdifactAgreementContent:
    properties: []
  EdifactOneWayAgreement:
    properties: []
  EdifactProtocolSettings:
    properties:
      envelopeOverrides:
        description: This is a default description.
        type: get
      messageFilterList:
        description: This is a default description.
        type: get
      schemaReferences:
        description: This is a default description.
        type: get
      validationOverrides:
        description: This is a default description.
        type: get
      edifactDelimiterOverrides:
        description: This is a default description.
        type: get
  EdifactValidationSettings:
    properties:
      validateCharacterSet:
        description: This is a default description.
        type: get
      checkDuplicateInterchangeControlNumber:
        description: This is a default description.
        type: get
      interchangeControlNumberValidityDays:
        description: This is a default description.
        type: get
      checkDuplicateGroupControlNumber:
        description: This is a default description.
        type: get
      checkDuplicateTransactionSetControlNumber:
        description: This is a default description.
        type: get
      validateEdiTypes:
        description: This is a default description.
        type: get
      validateXsdTypes:
        description: This is a default description.
        type: get
      allowLeadingAndTrailingSpacesAndZeroes:
        description: This is a default description.
        type: get
      trimLeadingAndTrailingSpacesAndZeroes:
        description: This is a default description.
        type: get
  EdifactFramingSettings:
    properties:
      serviceCodeListDirectoryVersion:
        description: This is a default description.
        type: get
      characterEncoding:
        description: This is a default description.
        type: get
      protocolVersion:
        description: This is a default description.
        type: get
      dataElementSeparator:
        description: This is a default description.
        type: get
      componentSeparator:
        description: This is a default description.
        type: get
      segmentTerminator:
        description: This is a default description.
        type: get
      releaseIndicator:
        description: This is a default description.
        type: get
      repetitionSeparator:
        description: This is a default description.
        type: get
  EdifactEnvelopeSettings:
    properties:
      groupAssociationAssignedCode:
        description: This is a default description.
        type: get
      communicationAgreementId:
        description: This is a default description.
        type: get
      applyDelimiterStringAdvice:
        description: This is a default description.
        type: get
      createGroupingSegments:
        description: This is a default description.
        type: get
      enableDefaultGroupHeaders:
        description: This is a default description.
        type: get
      recipientReferencePasswordValue:
        description: This is a default description.
        type: get
      recipientReferencePasswordQualifier:
        description: This is a default description.
        type: get
      applicationReferenceId:
        description: This is a default description.
        type: get
      processingPriorityCode:
        description: This is a default description.
        type: get
      interchangeControlNumberLowerBound:
        description: This is a default description.
        type: get
  EdifactAcknowledgementSettings:
    properties:
      needTechnicalAcknowledgement:
        description: This is a default description.
        type: get
      batchTechnicalAcknowledgements:
        description: This is a default description.
        type: get
      needFunctionalAcknowledgement:
        description: This is a default description.
        type: get
      batchFunctionalAcknowledgements:
        description: This is a default description.
        type: get
      needLoopForValidMessages:
        description: This is a default description.
        type: get
      sendSynchronousAcknowledgement:
        description: This is a default description.
        type: get
      acknowledgementControlNumberPrefix:
        description: This is a default description.
        type: get
      acknowledgementControlNumberSuffix:
        description: This is a default description.
        type: get
      acknowledgementControlNumberLowerBound:
        description: This is a default description.
        type: get
      acknowledgementControlNumberUpperBound:
        description: This is a default description.
        type: get
  EdifactMessageFilter:
    properties: []
  EdifactProcessingSettings:
    properties:
      maskSecurityInfo:
        description: This is a default description.
        type: get
      preserveInterchange:
        description: This is a default description.
        type: get
      suspendInterchangeOnError:
        description: This is a default description.
        type: get
      createEmptyXmlTagsForTrailingSeparators:
        description: This is a default description.
        type: get
      useDotAsDecimalSeparator:
        description: This is a default description.
        type: get
  EdifactEnvelopeOverride:
    properties:
      messageId:
        description: This is a default description.
        type: get
      messageVersion:
        description: This is a default description.
        type: get
      messageRelease:
        description: This is a default description.
        type: get
      messageAssociationAssignedCode:
        description: This is a default description.
        type: get
      targetNamespace:
        description: This is a default description.
        type: get
      functionalGroupId:
        description: This is a default description.
        type: get
      senderApplicationQualifier:
        description: This is a default description.
        type: get
      senderApplicationId:
        description: This is a default description.
        type: get
      receiverApplicationQualifier:
        description: This is a default description.
        type: get
      receiverApplicationId:
        description: This is a default description.
        type: get
  EdifactMessageIdentifier:
    properties:
      messageId:
        description: This is a default description.
        type: get
  EdifactSchemaReference:
    properties:
      messageId:
        description: This is a default description.
        type: get
      messageVersion:
        description: This is a default description.
        type: get
      messageRelease:
        description: This is a default description.
        type: get
      senderApplicationId:
        description: This is a default description.
        type: get
      senderApplicationQualifier:
        description: This is a default description.
        type: get
      associationAssignedCode:
        description: This is a default description.
        type: get
      schemaName:
        description: This is a default description.
        type: get
  EdifactValidationOverride:
    properties:
      messageId:
        description: This is a default description.
        type: get
      enforceCharacterSet:
        description: This is a default description.
        type: get
      validateEdiTypes:
        description: This is a default description.
        type: get
      validateXsdTypes:
        description: This is a default description.
        type: get
      allowLeadingAndTrailingSpacesAndZeroes:
        description: This is a default description.
        type: get
      trimLeadingAndTrailingSpacesAndZeroes:
        description: This is a default description.
        type: get
  EdifactDelimiterOverride:
    properties:
      messageId:
        description: This is a default description.
        type: get
      messageVersion:
        description: This is a default description.
        type: get
      messageRelease:
        description: This is a default description.
        type: get
      dataElementSeparator:
        description: This is a default description.
        type: get
      componentSeparator:
        description: This is a default description.
        type: get
      segmentTerminator:
        description: This is a default description.
        type: get
      repetitionSeparator:
        description: This is a default description.
        type: get
      releaseIndicator:
        description: This is a default description.
        type: get
      messageAssociationAssignedCode:
        description: This is a default description.
        type: get
      targetNamespace:
        description: This is a default description.
        type: get
  IntegrationAccountCertificateListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  IntegrationAccountCertificate:
    properties: []
  IntegrationAccountCertificateProperties:
    properties:
      createdTime:
        description: This is a default description.
        type: get
      changedTime:
        description: This is a default description.
        type: get
      metadata:
        description: This is a default description.
        type: get
      publicCertificate:
        description: This is a default description.
        type: get
  KeyVaultKeyReference:
    properties:
      keyVault:
        description: This is a default description.
        type: get
      keyName:
        description: This is a default description.
        type: get
      keyVersion:
        description: This is a default description.
        type: get
  IntegrationAccountSessionFilter:
    properties:
      changedTime:
        description: This is a default description.
        type: get
  IntegrationAccountSessionListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  IntegrationAccountSession:
    properties: []
  IntegrationAccountSessionProperties:
    properties:
      createdTime:
        description: This is a default description.
        type: get
      changedTime:
        description: This is a default description.
        type: get
  Operation:
    properties:
      name:
        description: This is a default description.
        type: get
  OperationListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  ErrorResponse:
    properties: []
  ErrorProperties:
    properties:
      code:
        description: This is a default description.
        type: get
      message:
        description: This is a default description.
        type: get
x-collection-name: Azure Logic Apps
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---