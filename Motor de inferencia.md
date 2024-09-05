# Motor de inferencia y explicación
class InferenceEngine:
    def __init__(self, knowledge_base):
        self.knowledge_base = knowledge_base

    def infer(self, symptom):
        for rule in self.knowledge_base.get_rules():
            if symptom in rule:
                return rule
        return "No se encontró ninguna regla para este síntoma."
