# python
from diagrams import Diagram
from diagrams.aws.storage import S3
from diagrams.onprem.compute import Server
from diagrams.aws.analytics import Redshift

with Diagram("My Design Diagram") :
    DataService = Server("Data Service")

    S3Storage = S3("S3 Bucket")

    MasterDB = Redshift("Redshift DW")
