# imagingtrack-testscripts

This repo contains test scripts used in : 
* [HL7 Connectathon 28](https://confluence.hl7.org/display/FHIR/2021+-+09+Connectathon+28) within the [imaging track](https://confluence.hl7.org/display/FHIR/2021-09+Imaging+Track)
* [HL7 Connectathon 29](https://confluence.hl7.org/display/FHIR/2022+-+01+Connectathon+29) within the [imaging track](https://confluence.hl7.org/display/FHIR/2022-01+Imaging+Track)

The repo contains 8 test scripts, related to [Radiation Dose Summary](https://hl7.org/fhir/uv/radiation-dose-summary/2022Jan/) testing, and [ImagingStudy](https://hl7.org/fhir/imagingstudy.html) testing. The scripts are related to three scenarios : 

* scenario 1: FHIR-enhanced Enterprise Viewer
    * FHIREnhancedViewerEndpointAccess.xml    : TestScript to simulate an EMR capacity to share ImagingStudy and Endpoint resources.
    * FHIREnhancedViewerRelatedResources.xml  : TestScript to simulate an EMR capacity to share ImagingStudy and its related resources.
    * FHIREnhancedViewerSearchParam.xml       : TestScript to simulate a viewer searching and retrieving ImagingStudy resources.
    * FHIREnhancedViewerAssociatedResources.xml : TestScript to simulate a viewer searching and retrieving associated resources with ImagingStudy resources.
* scenario 2: Radiation Dose Summary for Diagnostic Procedures on FHIR
    * RDSSharingVerification.xml  : TestScript to validate the sharing data between RDSP actor and a FHIR Server.
    * RDSPSimulator.xml           : TestScript to validate the FHIR Server capabilities against an RDSP actor.
    * RDSCSimulator.xml           : TestScript to validate the FHIR Server searching capabilities.
* scenario 3: Study Content Notification on FHIR
    * StudyContentNotification.xml : TestScript to simulate an Archive communicating ImagingStudy to EMR.