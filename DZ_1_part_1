from abc import ABC
import pickle
import json


from abc import ABC, abstractmethod


class SerializationInterface(ABC):
    @abstractmethod
    def save_to_file():
        pass


class SerializedJSON(SerializationInterface):
    def save_to_file(self, obj):
        with open("serialized.json", "w") as fh:
            json.dump(obj, fh)


class SerializedBIN(SerializationInterface):
    def save_to_file(self, obj):
        with open("serialized.bin", "wb") as fh:
            pickle.dump(obj, fh)
